## On-Screen Seek Buttons:
- Users can seek forward or backward by clicking on on-screen buttons.
- The seek step for both forward and backward actions is set to 10 seconds.

## Keyboard Controls:
- Keyboard shortcuts are implemented for seeking through media content.

## Screenshot:
![Screenshot](https://github.com/vishal7245/bounty1/blob/main/Screenshot%20from%202023-12-02%2020-07-18.png)

## Implementation
- Install videojs seek button plugin
```npm install videojs-seek-buttons```
- Implement the plugin

```
player.seekButtons({
            forward: 10,
            back: 10,
          })
 ```
- Use CDN for keyboard seek plugin
```<script src="https://cdn.sc.gl/videojs-hotkeys/0.2/videojs.hotkeys.min.js"></script>```

- Implement plugin
```
        player.hotkeys({
            seekStep: 10,
            enableVolumeScroll: true, 
            enableNumbers: false, 
            enableJogStyle: true 
        });```
