const CACHE_NAME = "schedulatore-cache-v1";
const urlsToCache = [
  "index.html",
  "manifest.json",
  "service-worker.js"
  // aggiungi eventuali altri file essenziali qui
];

// Install SW e cache iniziale
self.addEventListener("install", event => {
  event.waitUntil(
    caches.open(CACHE_NAME).then(cache => {
      return cache.addAll(urlsToCache);
    })
  );
});

// Attiva SW e aggiorna cache vecchie
self.addEventListener("activate", event => {
  event.waitUntil(
    caches.keys().then(keys =>
      Promise.all(
        keys.filter(key => key !== CACHE_NAME)
          .map(key => caches.delete(key))
      )
    )
  );
});

// Intercetta richieste e serve dalla cache se possibile
self.addEventListener("fetch", event => {
  event.respondWith(
    caches.match(event.request).then(response =>
      response || fetch(event.request)
    )
  );
});