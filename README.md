# polymer-uploader
A file uploader component for Polymer

## How to use ```polymer-uploader```?
Just import ```polymer-uploader``` and set up necessary properties:
- ```method```, set your HTTP request method
- ```url```, set the url where you want to hit

```
<polymer-uploader
  method="POST"
  url="YOUR_UPLOAD_URL">
</polymer-uploader>
```

- ```multiple```, Add it as a property if you want to upload multiple files together (optional)

```
<polymer-uploader
  uploading={{uploading}}
  method="POST"
  url="YOUR_UPLOAD_URL">
</polymer-uploader>
```

Listen to upload events:
- ```success```, True will be notified on upload success.
- ```uploading```, True will be notified while upload is going on.

```
<polymer-uploader
  multiple
  success={{success}}
  uploading={{uploading}}
  method="POST"
  url="YOUR_UPLOAD_URL">
</polymer-uploader>
```

## How to run the demo?
- Clone the repo
- Navigate to the repo using terminal
- Run ```bower install```
- Run ```polymer serve```
- Open your browser and go to ```your-polymer-development-url/demo```, (usually ```http://127.0.0.1:8081```)

### TBD
- Progress listener
- Nodejs file uploader for testing
