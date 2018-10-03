### Metric Imperial Converter : Documentation

*   End Point is
`GET /api/convert`
eg.
 `GET /api/convert?input=4km`

 returns `{"initNum":4,"initUnit":"km","returnNum":2.48548,"returnUnit":"mi","string":"4 kilometers converts to 2.48548 miles"}`

*   If unit and number are invalid or query parameter is other then "?input", return will be 'invalid unit'.
`/api/convert?input=12 or /api/convert?input=km12 or /api/convert?test=12km`

 returns
`invalid unit`

*   Fractions can be used, in query parameter (ie. 5, 1/2, 2.5/6), but if nothing is provided it will default to 1\.

#### Example Usage:

*   `/api/convert?input=4gal`
*   `/api/convert?input=1/2km`
*   `/api/convert?input=5.4/3lbs`
*   `/api/convert?input=kg`

#### Example Return:

`{"initNum":1,"initUnit":"km","returnNum":0.62137,"returnUnit":"mi","string":"1 kilometers converts to 0.62137 miles"}`