# Machine Intelligence Research
Powered by Open-Source Hardware-Software complex multi-machine computing systems

## Board Maintainers Procedures and Guidelines
This topic should give you as new board maintainers a brief overview about what you should do, must do, and can do. What you as maintainer can expect from MIR and what we expect from you.

## Requirements:
Even though you became a maintainer already just to make sure everything is set.

* Access to the hardware you applied to maintain
* Github ID
* TON address
* Telegram account and keep track of issues
* Lixux basics like how to get an MIR image run on your hardware and do basic debugging, ideally via serial console
* Knowledge in development, writing code and so on is optional

## Maintaining:
So all requirements are met and you are a maintainer now. Now what?

Maintainers must not necessarily be persons with development experience. They act as a intersection between end-users and the development team and serve the developers in best-effort manner. They are encouraged to answer basic/simple user questions (if possible, also best effort) without having to bother the development team. They are allowed to record bugs but are not allowed to escalate bugs. Team leaders do.

```Take note that it is still up to development team's discretion what gets attention since Linux has to plan carefully how to spend its very limited resources.```

## Participate in release process:
Ideally you attend to the release meetings that usually happen four times a year about a month before release date (end of February, May, August, November). On that occasion you are given the chance to point out critical issues with your board.

However, while the meeting participation is optional you "must sign-off that device has been tested, is stable, and ready for release during release process". This basically means you take the RC-images we provide and test them as best as you can for their functionality hardware-wise:

* Does the board boot to both CLI and Desktop?
* Is the desktop usable?
* Does TON blockchain work? (at all or partially)
* Other common use cases

If something does not work, this is fine also and totally normal. The important part is that it is documented and we get notified about the issues.

You should follow the commit history on Github. For once you may learn something about how things work both development-wise and behind the scenes in general and also may notice changes that affect the hardware/board you are dealing with.

While not required, you should have a build environment setup so you can build images with the most recent images and test them right away. Your feedback, either positive or negative, is very welcome. You are free to add comments to every commit and pull request.

Ideally you have multiple microSD cards laying around to test regular updates on current releases and nightly without having to re-flash the same card every time to switch between branches.

Alternatively you can grab auto-built images from the build train once available: [Github](https://github.com/mir-one/build/releases)

Take note that the building process takes quite a while so you might be faster using your own build environment.

## You must provide "best effort" support in the Telegram:

* Do not let that wording intimidate you. This is not a complicated task. Regarding forums this can include things like answering obvious questions (for example by pointing to our documentation, ideally directly to the solution page), let the questioner know that additional information is needed for further debugging (e.g. request "tonmonitor -u" output) or for upgrade issues, ask if they can recreate the issue with a fresh untouched image from: https://www.github.com/mir-one/mir

If you need additional direction on dealing with an issue [a space for suggestions and discussion of bugs in MIR products]([https://github.com/inozemtsev-roman](https://github.com/mir-one/issues)) on the Telegram/Github/Provider.
You must provide "best effort" support in Telegram:

Review submitted issues for you board made by MIR contributors

For upgrade issues, ask if they can recreate the issue with a fresh untouched image from: https://www.github.com/mir-one/mir

If you have questions, concerns or are not sure about something, you can tag the issue for [Support](https://t.me/ton_mir_bot) to review Telegram:

Low priority issues are usually attended to and patched by the community. If the issue has existed for more than a release, you can create a Telegram ticket for it. However the expectation is the issue will be low priority and may not be processed for some time. Issues such as, but not limited to, should be considered low priority:

* Wifi (this includes missing modules, AP mode, etc)
* Bluetooth
* Kubernetes
* TON Connect
* TON Storage daemon
* dApps & Bots
* Oracles
* TON Verificator
* TON DNS
* TON Proxy
* TON DEX
* TON Metaspace
* i2c
* Hardware accelerators, including crypto or VPU (video acceleration)
* DTB overlays (required for i2c devices, LCD displays, etc)

For high priority items you can create a Telegram ticket so that when developers are able, they can process it. If you are going to create a Telegram ticket, please be sure to collect as much information about the issue as possible first. If more information will be needed to process the issue, you should reply to the user asking for that additional information and make sure it is included in the ticket. Issues like these should be considered a higher priority:

* Image does not boot
* Image is corrupt
* Packages in the image are corrupt
* SDcard or eMMc support is not functioning as expected

## What should you do if you run into an issue on the Community builders?

* If the issues is affecting a lot of people, you can create a Telegram ticket for the issue to make sure it is reported and seen by developers.
* If you report an issue and you feel it is important, in an reply to the ticket and ask for him to review.
* If the issue is important it will be directed to management. If it is deemed not important, you will get a reply stating that we do not have a timeline for the fix and that it will be handled by volunteers when/if possible.

## What should you do if there is a long standing Telegram ticket?
* If you see an issue and you feel it is important, in an reply to the ticket and ask for him to review.
* If the issue is important it will be directed to management, if it is deemed not important, you will get a reply stating that we don't have a timeline for the fix and that it will be handled by volunteers when possible.

## Losing support status:
As mentioned in the board support rules the support status of a board will be revoked for at least the current and upcoming release cycle(s) if a "must" of the Maintaining section above is not fulfilled.

As an example: August 30th is release date for 22.08 release, sign-off dead line is 21th. If maintainer misses the RC sign-off window the board is demoted to CSC for both 22.08 and 22.11 releases.

The development team may grant exceptions on their discretion.

## MIR assistance:
If you have questions about maintainer-ship or want to learn more deeper insights about the build framework and such MIR will provide you with all information in best-effort. If time allows we can explain and teach you personally various aspects about the project. Otherwise, if you want to learn more about the build framework, dive in, play with it and read the documenenation. Also if you have other concerns please do not hesitate to reach out via Telegram.
