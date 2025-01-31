<p align="center">
  <a href="https://mux.com/">
    <img src="https://avatars.githubusercontent.com/u/16199997?s=200&v=4" alt="Mux Logo">
  </a>
</p>

# Mux Data Streaming Exports of Video Views

Mux Data can stream views for customers on Media plan to an Amazon Kinesis or Google Pub/Sub endpoint in the customer’s cloud account. Views are sent to Kinesis or Pub/Sub as they complete and are made available to customers to retrieve from the stream within about one minute after the view ends.

See our [Streaming Exports guide](https://docs.mux.com/guides/data/export-raw-video-view-data#stream-views-as-they-complete) for more information on setting up streaming exports of video views.

## Streaming Exports Versioning

As Mux Data adds new metrics, new versions of the protobuf specification are released. This repository always contains the most up-to-date specification. See our guide on [understanding the data fields](https://docs.mux.com/guides/data/export-raw-video-view-data#understand-the-data-fields) to see a full list of supported metrics.

### Version 7

Added new metric:

- `video_startup_failure`

### Version 6

Added new metric:

- `view_has_ad`

### Version 5

Added new event metadata for `request_canceled`, `request_failed`, and `request_completed` events.

### Version 4

Added new event metadata for `ad` (`adplay`, `adplaying`, etc) and `error` events.

### Version 3

Added new metrics:

- `custom_6`
- `custom_7`
- `custom_8`
- `custom_9`
- `custom_10`
- `view_dropped_frame_count`
- `view_drm_type`

### Version 2

Added new metric:

- `mux_embed`

### Version 1

Video View proto spec.
