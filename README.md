# Documentation for gapi.client
I don't know why Google doesn't have this somewhere. Perhaps they don't want us to use it... but hey, it's still useful, so I'm here to make it more useful.

## gapi.client.drive
### gapi.client.drive.files
#### gapi.client.drive.files.get
Usage:
```
gapi.client.drive.files.get({fileID:your_file_id}).then((response)=>{
      console.log(response.result);
});

response.result:{
  kind: "drive#file", 
  id: "some_id", 
  name: "some_name", 
  mimeType: "application/vnd.google-apps.drive-sdk.894862693076"
}
```
