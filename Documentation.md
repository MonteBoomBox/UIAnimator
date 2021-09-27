# UIAnimator - Documentation
A simple, and easy-to-use UI tweeting library for the Unity game engine.

## Prerequisites
Have the UIAnimator package installed and imported into your project.

### Precuation !!
UIAnimator is only compatible with UI Elements. It will not function on regular GameObjects.

## UIAnimator Script Usage
After importing the UIAnimator package into your project, there will be two folders created, the Editor folder and the UIAnimator folder.

![UIAnimator Folders Look](https://github.com/MonteBoomBox/UIAnimatorData/blob/main/images/UIAnimator-Folders.png)

If you already have an Editor folder, just move the UIAnimatorEditor script into it. Now inside the UIAnimator folder, you will a single script called UIAnimator. That is all you need in order to create your UI animations.

Just drag and drop the UIAnimator script on any component you have. Once you add the script to your UI element, it will look something like this

![UIAnimator Script Look](https://github.com/MonteBoomBox/UIAnimatorData/blob/main/images/UIAnimator-Script-Look.png)

## UIAnimator Script Documentation
Now that the script is on your UI component, let’s see what each field on the script does. Let’s first talk about the default fields.

1. **Is Open (Boolean, Important)**
    
    The IsOpen field determines whether the component should in the active or the inactive state in terms of the animation. This boolean is public and can be toggled from any other script. We’ll look into that later.
    
2. **Animate Time (Float, Important)**
    
    The Animate Time variable defines how fast or slow the animation should play. The higher the value, the faster the animation becomes. The range of the Animate Time variable is set between 1 and 40.
    
3. **Toggle Key (Enum)**
    
    The Toggle Key is a dropdown menu which lets you select on which key’s press, the animation should play. The animation will keep toggling for every selected key’s press.
    
    If you don’t want to use this feature, it is completely fine. Just set the Toggle Key to “None”. For triggering the animation from any other script, just access the UIAnimator of that UI object and call the ToggleOpen() method. This will perform the same action which the Toggle Key does.
    
4. **Rect (RectTransform, Extremely Important)**
    
    This field lets you input any Rect Transform component. (preferably the one attached to the same object as this script) This field is extremely important as the animations related to Position, Rotation, and Scale cannot be performed if no Rect Transform is provided.
    
5. **Image (RectTransform, Extremely Important for Color Animation)**
    
    This field lets you input any Image component. (preferably the one attached to the same object as this script) This field is **extremely important** as the animations related to Color cannot be performed if no Image is provided.

---
Now to the fun stuff which is the Animation fields. These are the fields where you can define the actual animation parameters. And, it is incredibly easy to combine multiple animation types. For each animation type you want to use, just enable that specific Animation. (For ex. A Position and Scale Animation at the same time)

1. **Animate Position (Animates the position of the UI element)**

![Position Field Image](https://github.com/MonteBoomBox/UIAnimatorData/blob/main/images/Position-Field.png)

For animating the Position of the UI element, check the Animate Position box. Once you enable “Animate Position”, there will be 2 Vector2 fields which will popup.

In the “Start Position” field, you can set the beginning position of the UI element. In the “End Position” field, you can set the ending position of the UI element.

2. **Animate Rotation (Animates the rotation of the UI element)**

![Rotation Field Image](https://github.com/MonteBoomBox/UIAnimatorData/blob/main/images/Rotation-Field.png)

For animating the Rotation of the UI element, check the Animate Rotation box. Once you enable “Animate Rotation”, there will be 2 float fields which will popup.

In the “Start Rotation” field, you can set the beginning rotation of the UI element. In the “End Rotation” field, you can set the ending rotation of the UI element.

3. **Animate Scale (Animates the scale of the UI element)**

![Scale Field Image](https://github.com/MonteBoomBox/UIAnimatorData/blob/main/images/Scale-Field.png)

For animating the Scale of the UI element, check the Animate Scale box. Once you enable “Animate Scale”, there will be 2 Vector2 fields which will popup.

In the “Start Scale” field, you can set the beginning scale of the UI element. In the “End Scale” field, you can set the ending scale of the UI element.

4. **Animate Color (Animates the color of the UI element’s image)**

![Color Image Field](https://github.com/MonteBoomBox/UIAnimatorData/blob/main/images/Color-Field.png)

For animating the Color of the UI element’s Image, check the Animate Color box. Once you enable “Animate Color”, there will be 2 Color fields which will popup.

In the “Start Color” field, you can set the beginning color of the UI element’s Image. In the “End Color” field, you can set the ending color of the UI element’s Image.

---

### Conclusion

That is the complete documentation of UIAnimator!

If you have any more questions or suggestions, you can always create an issue about it on the GitHub page.

### P.S Developer Note
Hey there, I am Manas Joshi (MonteBoomBox), the creator of UIAnimator. I just wanted to give you a huge thank you for downloading this Unity library. It means a lot to me. 

### You are awesome!
