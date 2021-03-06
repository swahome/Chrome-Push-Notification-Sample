# Push Notifications demo

## Setup

You will need:

* Google Cloud Messaging `Project ID` and an `Authorization Key`
* You will also need the `Device ID` from the Browser you will be Using

The Pushing Requires a cURL command from Your Console.

````SH

    curl --header "Authorization: key=<AUTH-KEY>" --header "Content-Type: application/json" https://android.googleapis.com/gcm/send -d "{\"registration_ids\":[\"<DEVICE-ID>\"]}"

````

Also Remember to Update Your `manifest.json` to set your Project ID`.

````JS

    {
      "name": "Push Notifications codelab",
      "gcm_sender_id": "<PROJECT-ID>"
    }

````

## License

Copyright 2015 Google, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor license agreements. See the NOTICE file distributed with this work for additional information regarding copyright ownership. The ASF licenses this file to you under the Apache License, Version 2.0 (the “License”); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an “AS IS” BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

Please note: this is not a Google product
