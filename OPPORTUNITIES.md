# AsTeR - Opportunities

`Author: Meryll Dindin`

![LOGO](./assets/aster-whitened.png)

**AsTeR** is a platform used by emergency call centers to **collect**, **analyze** and **prioritize** information. AsTeR brings state-of-the-art machine learning and modularized software for emergency response. Better information can help first responders respond to emergencies in a more efficient manner. Via a range of services ranging from call analysis to video streaming, AsTeR allows first responders to visualize the emergency and mentally prepare for it. In addition, AsTeR’s prioritization tool allows for efficient triage of calls. This is especially helpful during natural disasters when resources run scarce and emergency call centers are overwhelmed.

Ultimately, AsTeR is an open-source project built for the design of a **modular audio streams analysis backend**. We aim at expanding the scope of the edge technology deployed by a few to help many. As such, the core will is to keep intrinsic modularity and flexibility all along the development of this project, and see it used in an impactful way. To make AsTeR a reality, our team is closely working with emergency responders while conducting a wide range of interviews to understand the current pain points when responding to mass casualty incidents.

Learn more about our projects on:

* [Medium](https://towardsdatascience.com/project-aster-ibm-call-for-code-30d959614be7)
* [Press Releases](https://www.project-aster.com/press)
* [Youtube](https://youtu.be/fLeLd2vp-8g)

## Projects

* [**website**](https://github.com/Project-AsTeR/website): Host the current web platform (Flask, HTML, CSS and JS), presenting the project as well as the roadmap for the vision. The website also host a working demo of our core product, and will highly likely also host the web-hosted platform for our users.
* [**stream**](https://github.com/Project-AsTeR/stream): Core Docker container absorbing the incoming stream of emergency calls from a Twilio endpoint, over a secured websocket. Concurrent threads are also hosted on this service, to retrieve call specific meta-data, converting audio-files from ULAW to WAV, and running real-time transcription with an AWS endpoint.
* [**trigger**](https://github.com/Project-AsTeR/trigger): Build the lambda function triggered by SQS events everytime a new call is streamed to our platform. It aims at doing the transcriptions and the analysis (by calling our scoring endpoint).
* [**scoring**](https://github.com/Project-AsTeR/scoring): Core service aimed at attributing priority to an incoming transcript. It also uses NLU for emotion analysis, and keywords extraction. It corresponds to the instance deploying the deep learning models fine-tuned on the desired problematics.
* [**bastion**](https://github.com/Project-AsTeR/bastion): With such an explicit name, this service is a back-up instance aimed at being poped-up to proxy with the internal services of our VPC, in order to avoid to be locked out due to security issues.

## Impact

The current beta version of AsTeR focusses on triaging 911 phone calls, extracting key information and making it readily available for first responders via an interactive map. The map helps identify high priority zones. Project AsTeR is currently backed by key players in the field including **IBM**, **Ovio**, the **Clinton Global Initiative**, the **American Red Cross**, the **United Nations** and the **Linux Foundation**. AsTeR’s goal is to become the centralized platform for information during natural disasters. Phone calls are just the start; drones, social media, news agencies are amongst the next sources of information we are targeting. Join us on this incredible adventure and help AsTeR save lives.

## Current Used Technology

![LOGO](./assets/aster-v0.png)

## Sought Skills

Due to the concrete amount of possibilities, here are the multiple profiles that would have a great impact on the project:

* _Front_: HTML, CSS, JS
* _Back_: Python, Tensorflow, PyTorch, NLP, Audio Analysis
* _Infra_: MySQL, Docker, WebSockets, AWS, Twilio, MapBox, Kubernetes, Terraform, Continuous Integration

## Currently Heading Towards

![LOGO](./assets/aster-v1.png)

## Get in Touch

Contact us at aster.messages@gmail.com and we will get back to you as soon as possible!
