# Naturherzen Formunauts/DonutApp Integration

## Requirements

* PHP v7.0+
* CiviCRM (``5.3.28+``)
* DonutApp Extension (``at.greenpeace.donutapp`` ``v1.4+``)
* XCM Extension (``at.systopia.xcm`` ``v1.8+``)

## Installation

1. Install the required extensions (XCM + DonutApp)
1. Install this extension
1. Create and configure an XCM profile called ``donutapp``.
2. Create an hourly scheduled job for ``DonutDonation.import`` with the following parameters: 
```
client_id=<formuauts_client_id>
client_secret=<formuauts_client_secret>
campaign_id=<campaign_id>
processor=Naturherzen
confirm=1
limit=20
```