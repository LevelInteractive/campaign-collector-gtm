# Campaign Collector

<img src="assets/tpl-overview.png" width=830 style="margin: 0 auto; display: block;" />

---

This tag template is a wrapper around the main CampaignCollector.js library and provides a simplified interface for users to configure the library without having to utilize Custom HTML/JS code to do so. 

> [!IMPORTANT]
> For a full README on what this tag does. Please see the main [CampaignCollector.js](https://github.com/LevelInteractive/campaign-collector) library.

### Permissions

#### Injects Scripts
This tag template loads Level's [CampaignCollector](https://github.com/LevelInteractive/campaign-collector) library through the [jsDelivr.com](https://www.jsdelivr.com/) CDN.

#### Accesses Global Variables

- The template will write/read/execute to a `_campaignCollector` global variable, and several sub-properties of it. 
- The template will access the `CampaignCollector.create` method to initialize a the library on the `_campaignCollector` global mentioned above.
- The template will access the `CampaginCollector.consentChange` method to emit an event to the instances to handle changes in consent state for `ad_storage`, `analytics_storage`, `ad_user_data`, `ad_personalization`

## Reads Consent State

The template will listen/read the consent state for the following types:  `ad_storage`, `analytics_storage`, `ad_user_data`, `ad_personalization`.

### Author(s)
[@derekcavaliero](https://github.com/derekcavaliero)
