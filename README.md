# Splunk_TA_bro_patched

Patches the Splunk_TA_bro that comes installed on logger within DetectionLab to apply tags, eventtypes and sourcetype splitters.

With the exception of field extractions, all other knowledge objects are dependant on the sourcetype being `sourcetype=bro:json`, whereas the sourcetype in DetectionLab is `sourcetype=zeek:json`.

## Changes

Changes made under /local/ from bro to zeek:

 - eventtypes.conf remapped 
 - props.conf remapped
 - tags.conf remapped
 - transforms.conf remapped
 - lookups/* remapped & fields renamed

![image](https://user-images.githubusercontent.com/56516924/162644220-cf4d1afa-444d-48e9-96b2-e308239ea6b0.png)

![image](https://user-images.githubusercontent.com/56516924/162644327-77c0fa72-e2a4-4582-9c7e-6f45c3a425ca.png)


## Acknowledgements

Original TA is created by Splunk and can be found on Splunkbase - https://apps.splunk.com/app/1617/.  It has not been updated since Dec 2018.
