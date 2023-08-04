# messier-api
###### by Osric Dienda
Messier catalog API that provides data and images for all 110 Messier objects. 
<br>
To download for Node.js, run:

```bash
$ npm install messier-api
```
&nbsp;

After installing the package, import the library using `require` or `import`.

```js
const messier = require('messier-api');
```
&nbsp;

To access data on the Messier objects, access `messier.data` or use `messier.getMessier()`.

```js
console.log(messier.data.M45.name);
```
```js
console.log(messier.getMessier(45).name);
```
&nbsp;

### Messier object attributes:
| Attribute | Description | Code Example |
| ----------|-------------|--------------|
| messierNumber | The Messier number of the object. | `messier.data.M45.messierNumber` |
| name | The common name of the Messier object. If none exists, NGC number or description is used instead. | `messier.data.M45.name` |
| alternateNames | An array of the object's alternate names. Most have no alternate names (empty array). | `messier.data.M45.alternateNames` |
| NGC | The New General Catalog (NGC) or Index Catalog (IC) of the Messier object. Some objects have none (undefined). | `messier.data.M45.NGC` |
| type | Classifies objects into 12 different types: `Diffuse Nebula, Double Star, Elliptical Galaxy, Globular Cluster, Group/Asterism, Irregular Galaxy, Lenticular (S0) Galaxy, Open Cluster, Planetary Nebula, Spiral Galaxy, Star Cloud, Supernova Remnant`. | `messier.data.M45.type` |
| constellation | The name of the constellation the Messier object is in. | `messier.data.M45.constellation` |
| rightAscension | The right ascension of the Messier object. (hh:mm:ss.ss) | `messier.data.M45.rightAscension` |
| declination | The declination of the Messier object. (±dd:mm:ss.ss) | `messier.data.M45.declination` |
| magnitude | The apparent magnitude of the Messier object. | `messier.data.M45.magnitude` |
| size | The apparent dimensions of the Messier object in arcminutes (W' x H'). If elliptical, only the angular diameter is given (D'). | `messier.data.M45.size` |
| distance | The distance of the Messier object from Earth in light-years. | `messier.data.M45.distance` |
| viewingSeason | The best season to view the Messier object from the Northern Hemisphere. | `messier.data.M45.viewingSeason` |
| viewingDifficulty | How hard it is to view the Messier object, classified as either: `Very Easy, Easy, Moderate, Hard, Very Hard`. | `messier.data.M45.viewingDifficulty` |
