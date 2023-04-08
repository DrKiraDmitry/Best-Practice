# new URLSearchParams


Make a **GET** request, we need to create a URL with parameters and a common mistake is to create search parameters with **concatenation**

> '/getinfo?deliverypay=' + id + '&target_lat=' + (targetLat || '') + '&target_lon=' + (targetLon || '');

But you need a lot of conditions to create these URL search parameters

We can make things easier by using **new URLSearchParams**.

>'/get information?' + new parameters URLSearchParams({
> <br/>delivery: id,
> <br/>target_lat: targetLat,
> <br/>target_lon: targetLon
> <br/>});

This URLSearchParams gets the properties of the key-value type object, and if the key-value is empty, it will not create parameters.

And it will make your **code easier** and **more readable**.