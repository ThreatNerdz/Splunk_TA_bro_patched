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

![image](https://user-images.githubusercontent.com/56516924/162644486-e2f81b7d-914b-4220-b074-828462e4a66f.png)


## Acknowledgements

Original TA is created by Splunk and can be found on Splunkbase - https://apps.splunk.com/app/1617/.  It has not been updated since Dec 2018.
