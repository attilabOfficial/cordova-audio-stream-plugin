<!---
 license: Licensed to the Apache Software Foundation (ASF) under one
         or more contributor license agreements.  See the NOTICE file
         distributed with this work for additional information
         regarding copyright ownership.  The ASF licenses this file
         to you under the Apache License, Version 2.0 (the
         "License"); you may not use this file except in compliance
         with the License.  You may obtain a copy of the License at

           http://www.apache.org/licenses/LICENSE-2.0

         Unless required by applicable law or agreed to in writing,
         software distributed under the License is distributed on an
         "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
         KIND, either express or implied.  See the License for the
         specific language governing permissions and limitations
         under the License.
-->

# cordova-audio-stream-plugin

Basic cordova media plugin not allow to play radio audio stream on ios.
This cordova plugin allow you to read a live radio stream

The android part of this plugin is from https://github.com/apache/cordova-plugin-media, I don't modify it

#Installation
Run 
    cordova plugin add https://github.com/keosuofficial/cordova-audio-stream-plugin.git
    
#Use it
    my_stream = new Stream("http://your_live_radio_streeam", onSuccess, onError);
    // Play audio
    my_media.play();
    function onSuccess() {
        console.log("playAudio():Audio Success");
    }
    function onError(error) {
        alert('code: '    + error.code    + '\n' +
        'message: ' + error.message + '\n');
    }

You can also stop the music with
    my_media.stop();
