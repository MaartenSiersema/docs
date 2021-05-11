---
id: visor
title: Visor
sidebar_label: Visor
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

### Learn about using Visor 
The Deta Visor offers a user interface for you to see a live view of all the events processed by your Micro. You can use it to monitor and debug your requests, test your endpoints by sending requests, and more.
### Opening Visor
<Tabs 
    defaultValue="browser" 
    values={[
    { label: 'Browser', value: 'browser' },
    { label: 'Terminal', value: 'terminal' },
    ]
}>
<TabItem value="browser">

Start by logging into your console at [deta.sh](https://deta.sh). You should be redirected to the following screen:

<img src="/img/visor/visor_1.png" alt="visor_1" width="800"/>

Once that's done, choose a micro to view by clicking on its name (under the _"Micros"_ tab).

<img src="/img/visor/visor_2.png" alt="visor_2" width="800"/>

Now click on _"Visor"_

<img src="/img/visor/visor_3.png" alt="visor_3" width="800"/>

</TabItem>
<TabItem value="terminal">

Start your terminal in the root directory of your deployed Deta project.

Run `deta visor open`.

</TabItem>
</Tabs>

### Navigating the Visor
The Visor page has the link to your Micro in the top right, a button named _"HTTP Client"_ in the bottom left, and a list of all the events handled by your Micro!

<img src="/img/visor/visor_4.png" alt="visor_4" width="800"/>

#### The Event List
The Visor logs every single event made to your Micro, each event has the **HTTP Status Code**, the **HTTP Method**, and the **time** logged above it. Under this information are three tabs, letting you view the response, request, and logs of the event. 

Response:
<img src="/img/visor/visor_5.png" alt="visor_9" width="800"/>

The Request sent to the Micro:

<img src="/img/visor/visor_6.png" alt="visor_10" width="800"/>

And logs (normally displaying errors if they were to occur):

<img src="/img/visor/visor_7.png" alt="visor_11" width="800"/>

On the top right of every event are two icons:

<img src="/img/visor/visor_8.png" alt="visor_12" width="800"/>

The _"pen"_ icon lets you edit the request before re-sending it to your micro and the _"redo"_ icon lets you send the same request again.


#### The HTTP Client
Visor also has a built in _"HTTP Client"_ to make requests to your Micro. You can use this by clicking on the _"HTTP Client"_ button. 

<img src="/img/visor/visor_13.png" alt="visor_6" width="600"/>

Simply specify the request method, path, headers and body and hit the _"Send"_ button to send it off!

<img src="/img/visor/visor_14.png" alt="visor_7" width="600"/>

The content-type can be changed from JSON to Text, using the selection box on the bottom left of this window.

<img src="/img/visor/visor_15.png" alt="visor_8" width="600"/>


### Video overview
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/kAwV7-bEtb0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
