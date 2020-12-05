# Little Drummers LookIt support files. 
### Created by Caspar Addyman <c.addyman@gold.ac.uk> 
#### Goldsmiths, University of London, 2020

_Version - Not even alpha!_

This folder contains files to run a web based study of rhythm perception in toddlers. The experiment runs on the 
[MIT LookIt](https://lookit.mit.edu) platform. To find out more about using this in your own research visit the [LookIT documentation](https://lookit.readthedocs.io/en/develop/).

The `proctocol.json` file tells the LookIt experiment runner what sequence of pages to show in what order.

```    "sequence": [
        "video-config",
        "video-consent",
        "first-instructions",
        "test-trials",
        "my-exit-survey"
    ]```

The current experiment consists of the following screens. 
 1. `video-config` -Standard LookIt camera set up instructions.
 2. `video-consent` The consent document is based on [Lookit consent form template 5.md](https://github.com/lookit/research-resources/blob/master/Legal/Lookit%20consent%20form%20template%205.md]. We set all the values we need for `PIName`, `purpose`, etc.
 Participants record a video statement that they've read the consent document
 3. `first-instructions` - Instructions specific for this study. It's very simple so we only need one page.
 4. `test-trials` - The experiment itself. We use `"sampler": "random-parameter-set"` with two different `parameter-sets` to show the tempo trials in two orders.  
   4.1.1 `SpontaneousMotorTempo.mp4` - silent video with instructions for parent to encourage child to drum on table (video recording - 30seconds)  
   4.1.2 `AttentionGetter1.mp4` (no recording - 5 seconds)  
   4.2.1  `400ms.mp4` - hand tapping table every 400 milliseconds (150bpm) (video recording - 20 seconds)  
   4.2.2 `AttentionGetter2.mp4` (no recording - 5 seconds)  
   4.3.1  `600ms.mp4` - hand tapping table every 400 milliseconds (100bpm) (video recording - 20 seconds)  
   4.3.2 `AttentionGetter3.mp4` (no recording - 5 seconds)  
   4.4.1  `500ms.mp4` - hand tapping table every 400 milliseconds (120bpm) (video recording - 20 seconds)  
   4.4.2 `AttentionGetter4.mp4` (no recording - 5 seconds)  
   4.5.1  `700ms.mp4` - hand tapping table every 400 milliseconds ( 86bpm) (video recording - 20 seconds)  
   4.5.2 `AttentionGetter5.mp4` (no recording - 5 seconds)  
   4.6.1  `SpontaneousMotorTempo.mp4` - silent video with instructions for parent to encourage clapping (video recording - 30seconds)  
   4.6.2 `AttentionGetter1.mp4` (no recording - 5 seconds)  
 5. `my-exit-aurvey` Thank you, debrief and exit to our Qualtrics survey.  


