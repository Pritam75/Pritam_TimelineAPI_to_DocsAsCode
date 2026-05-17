# Example Timeline Response

```json
{
    "summary_data": {
        "session_start_timestamp_ms": 1760583631583,
        "session_end_timestamp_ms": null,
        "play_status": "Joined and Ongoing",
        "client_id": "1234567890",
        "session_id": 0987654321,
        "required_tags": {
            "media_player_framework_name": "Exoplayer",
            "device_type": "Desktop",
            "c3.cm.episodeNumber": "1",
            "c3.cm.seriesName": "Iron Man",
            "device_category": "Web",
            "device_operating_system_family": "macOS",
            "c3.cm.name": "CMS",
            "c3.cm.showTitle": "The one with all characters",
            "c3.cm.brand": "Marvel",
            "browser_version": "Chrome 141.0.0.0",
            "c3.app.version": "5.0",
            "media_player_framework_version": "Exoplayer 7.3",
            "c3.cm.genre": "Action",
            "c3.viewer.id": "view",
            "content_length_ms": "1505000",
            "c3.cws.sf": "7",
            "c3.protocol.level": "2.6",
            "device_model": "Mac",
            "device_os": "macOS",
            "c3.player.name": "Android Exoplayer",
            "device_brand": "Chrome",
            "c3.cm.id": "40010",
            "asset": "Content",
            "c3.device.usesSdk": "T",
            "stream_url": "http://<url value>",
            "c3.video.isAd": "F"
        },
        "custom_tags": {
            "serialName": "false",
            "c3.cm.genretype": "Action, Romedy",
            "videoType": "VoD",
            "c3.cm.longUtmTrackingUrl": "googlecom",
            "streamProtocol": "HLS",
            "expireDate": "28 October 2031",
            "videoResolution": "1080 X 1000"
        },
        "video_start_time_ms": 19,
        "playing_time_ms": 11477,
        "paused_time_ms": 0,
        "rebuffering_time_ms": 0,
        "connection_induced_rebuffering_time_ms": "0",
        "average_peak_bitrate_bps": 320,
        "average_framerate_fps": 0,
        "average_average_bitrate_bps": 0,
        "is_exit_before_video_start": "false",
        "is_video_start_failure": "false",
        "is_video_playback_failure": "false",
        "is_video_start_failure_business": "false",
        "is_video_playback_failure_business": "false",
        "is_video_start_failure_tech": "false",
        "is_video_playback_failure_tech": "false"
    },
    "timeline_data": {
        "session_state": [
            {
                "start_time_ms": 1760583631599,
                "end_time_ms": 1760583631601,
                "value": "Unknown"
            },
            {
                "start_time_ms": 1760583631601,
                "end_time_ms": 1760583631602,
                "value": "Buffering"
            },
            {
                "start_time_ms": 1760583631602,
                "end_time_ms": 1760583635000,
                "value": "Playing"
            }
        ],
        "session_event": [
            {
                "time_ms": 1760583631583,
                "value": "SessionStart"
            },
            {
                "time_ms": 1760583631602,
                "value": "Play"
            }
        ],
        "session_overview_event": [
            {
                "time_ms": 1760583631602,
                "value": "Play"
            }
        ],
        "bitrate": [
            {
                "start_time_ms": 1760583631602,
                "end_time_ms": 1760583635000,
                "start_value": 320.0,
                "end_value": 320.0
            }
        ],
        "framerate": [],
        "connection_type": [
            {
                "start_time_ms": 1760583631583,
                "end_time_ms": 1760583635000,
                "value": "2G"
            }
        ],
        "cdn": [
            {
                "start_time_ms": 1760583631583,
                "end_time_ms": 1760583635000,
                "value": "AKAMAI"
            }
        ],
        "asset": [
            {
                "start_time_ms": 1760583631583,
                "end_time_ms": 1760583635000,
                "value": "Content"
            }
        ],
        "error": [],
        "custom_event": []
    }
}
```
