# p_fff_nachfuehrung

## Abbaustellen
```
java -jar /Users/stefan/apps/ili2gpkg-4.3.1/ili2gpkg-4.3.1.jar \
--dbfile afu_abbaustellen_fff.gpkg \
--defaultSrsCode 2056 --createGeomIdx --createFk --createFkIdx --createUnique --createEnumTabs --beautifyEnumDispName --createMetaInfo --createNumChecks --nameByTopic --strokeArcs \
--models SO_ALW_FFF_Uebersteuerung_20210528 --modeldir ".;http://models.geo.admin.ch" \
--schemaimport
```

```
java -jar /Users/stefan/apps/ili2gpkg-4.3.1/ili2gpkg-4.3.1.jar \
--dbfile afu_abbaustellen_fff.gpkg \
--models SO_ALW_FFF_Uebersteuerung_20210528 --modeldir ".;http://models.geo.admin.ch" \
--export afu_abbaustellen_fff.xtf
```

## Gewässerraum
```
java -jar /Users/stefan/apps/ili2gpkg-4.3.1/ili2gpkg-4.3.1.jar \
--dbfile alw_gewaesserraum.gpkg \
--defaultSrsCode 2056 --createGeomIdx --createFk --createFkIdx --createUnique --createEnumTabs --beautifyEnumDispName --createMetaInfo --createNumChecks --nameByTopic --strokeArcs \
--models SO_ALW_Gewaesserraum_20210531 --modeldir ".;http://models.geo.admin.ch" \
--schemaimport
```

```
java -jar /Users/stefan/apps/ili2gpkg-4.3.1/ili2gpkg-4.3.1.jar \
--dbfile alw_gewaesserraum.gpkg \
--models SO_ALW_Gewaesserraum_20210531 --modeldir ".;http://models.geo.admin.ch" \
--export alw_gewaesserraum.xtf
```

## todo
- Deploy Übersteuerungsmodell
- Abbaustellen
  * In Edit-DB anlegen
  * Export nach S3 