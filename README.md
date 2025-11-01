# kookadvies

Advice to boil water 2025-11-01 in area: https://bertt.github.io/kookadvies/

News: https://www.vitens.nl/Storing-en-onderhoud/Kookadvies-drinkwater


## Method

Source data dowload pc4: https://public.opendatasoft.com/explore/assets/georef-netherlands-postcode-pc4/export/

Select subset of postcode areas and convert to GeoJSON

```
ogr2ogr -f GeoJSON filtered_postcodes.geojson georef-netherlands-postcode-pc4.fgb -where "pc4_code IN ('3511','3512','3513','3514','3515','3521','3522','3523','3524','3525','3526','3527','3528','3531','3532','3533','3534','3541','3542','3551','3552','3553','3554','3555','3561','3562','3563','3564','3565','3566','3571','3572','3573','3581','3582','3583','3584','3585','3602','3611','3612','3615','3704','3721','3722','3723','3731','3732','3735','3737','3981')" -select pc4_code
```

Visualisation in MapLibre, background map https://openfreemap.org/
