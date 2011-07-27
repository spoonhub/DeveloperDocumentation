# API Method: /api/liveevent/stream/record
# flags=comments

Start recording from a live event video stream


### Parameters

<table class="pretty">
  <tr><th>Parameter</th><th>Description</th></tr>
  <tr><td><tt>liveevent_stream_id</tt> <small>(required)</small></td><td>The ID for the stream for which you want to record.</td></tr>
</table>

    

### Permission level 

The minimum required [permission level](index#permission-level) is:

    write


### Example XML Response

    <response status="ok" permission_level="write" 
      message="The stream has started recording" cached="0">

### Example JSON Response

    {
      "status": "ok", 
      "message":"The stream has started recording",
      "permission_level":"write",
      "cached":"0",
      "p": "1",
      "size": "1",
      "site": { ...},
      "endpoint": "/api/liveevent/stream/start"
    }