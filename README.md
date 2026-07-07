# Pipe Video Recorder Widget for Jotform

A custom Jotform widget that loads _JotFormCustomWidget.min.js_ and _Pipe Recording Client_, embedding a video recorder into a form. Users can record a video or upload a video file directly from the form, and the resulting recording URL is submitted as the field's value.

Use this widget to:

- Collect video responses, testimonials, applications, interviews, and feedback;
- Upload existing video files;
- Configure the recorder’s dimensions and maximum recording duration;
- Connect the widget using your Pipe account hash and environment ID.

## Widget Settings

These are the settings configured in the Jotform widget settings panel:

| Setting            | Description                                    | Default        |
|--------------------|------------------------------------------------|----------------|
| `accountHash`      | Your addpipe.com account hash                  | —              |
| `eid`              | Pipe environment ID                            | —              |
| `qualityUrl`       | Recording quality profile XML                  | `avq/480p.xml` |
| `pipeWidth`        | Recorder width (px)                            | `640`          |
| `pipeHeight`       | Recorder height (px)                           | `480`          |
| `maxRecordingTime` | Max recording time (seconds)                   | `600`          |

## Output Value

On success, the field value is a constructed URL of the form:

````
https://<location>/<accountHash>/<fileName>.mp4
````

## File Structure

This widget is a single self-contained HTML file with inline CSS/JS references to the external Jotform and Pipe SDKs. 

## Requirements

- An [addpipe account](https://dashboard.addpipe.com/signup) (for accountHash and eid);
- A Jotform form with this **Pipe Video Recorder** widget.

## Other Links: 
- [https://blog.addpipe.com/capturing-videos-with-pipe-in-a-jotform-contact-form/](https://blog.addpipe.com/capturing-videos-with-pipe-in-a-jotform-contact-form/)
