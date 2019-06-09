# Documentation for gapi.client
I don't know why Google doesn't have this somewhere. Perhaps they don't want us to use it... but hey, it's still useful, so I'm here to make it more useful.

## gapi.client.drive
### gapi.client.drive.files
#### gapi.client.drive.files.get
Note: YOU NEED TO INCLUDE A .then((r)=>{}) OR YOUR METHOD WILL NOT WORK
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
#### gapi.client.drive.files.update
Note: YOU NEED TO INCLUDE A .then((r)=>{}) OR YOUR METHOD WILL NOT WORK
Usage:
```
gapi.client.drive.files.update({fileID:your_file_id, resource:{metadata}}).then((response)=>{
      console.log(response.result);
});

response.result:{
  kind: "drive#file", 
  id: "some_id", 
  name: "some_name", 
  mimeType: "application/vnd.google-apps.drive-sdk.894862693076"
}
```
