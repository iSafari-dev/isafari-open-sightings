# iSafari Open Sightings

A planned open dataset of verified wildlife sightings from safari guides in Kenya, stored on Filecoin with IPFS CIDs.

iSafari is a wildlife app, live on Google Play (https://play.google.com/store/apps/details?id=com.isafari). Guides upload a photo or video, the app saves the GPS point and capture time, and the species is identified automatically. A sighting is created only if the point is inside a known park and the species is recognized. Anything else goes to an admin review queue.

Today those records sit in our private database. This repo is where we will publish them as open data.

## What the dataset will contain

For each reviewed sighting:

- Sighting ID
- Species common and scientific name
- Park or conservancy
- Location rounded to about 1 km
- Capture date and time
- How it was checked (automatic rules or admin review)
- Photo CID on Filecoin/IPFS

Records will be published as JSON and CSV, with a monthly manifest file that has its own CID.

## Protecting sensitive species

Poaching is a real risk. Exact coordinates are never published. Locations are rounded to about 1 km for most species, and for sensitive species like rhino the location is withheld or reduced to the park level.

## Status

Planning stage. No data or code here yet. App code stays in our private repos.

## License

Dual licensed under MIT or Apache-2.0, at your option. See LICENSE-MIT and LICENSE-APACHE.
