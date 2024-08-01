# FEATURES:

## PROBLEM:
When visiting the site in a Desktop PC, Ar button doesn't show as it is a movile feature only.
This solution doesn't impact the overall experience, unless the user opens up the site on its movile device.

## INITIAL SOLUTION: 
Provide a QR (that only shows in desktop) that let's user to acces the model with their movile devices.

## ISSUES:
As explained by [Elalish](https://github.com/google/model-viewer/discussions/2933#discussioncomment-1554375), in order to work user need to download the 3d asset in it's device (this happens every time a user visits the site).
Because downloading something without seeing first is an universal hazard, it's not useful try hack a way around.

## BRAINSTORMING:

1. A QR code to the same page, maybe with the #id of the 3D model.
    - ✔️ Easy to implement. No extra development needed.️ 
    - ❌ It's not straight-foward, or at least in the best case, users needs to look for the Ar button for themselves.
      - 💡 A script could be set on place, to trigger some CTA to prompt users to use the AR button whenever someone enters the site through that particular url. 
      
2. To have a dedicated page for each model, that when visiting that URL allows to download the model and then prompting the user to click the AR button.
    - ✔️ It can improve user experience by using this dedicated space to add tips to help new users use this feature.
    - ❌ It will be needed to code an extra page for each model.
      - 💡 Since 3D assets are not embedded on each page, it's possible to resolve this with a dynamic page wich loads the model's id (reducing N to 1 development).

## PRODUCTION:

### Tasks:
- [ ] Solution 1:
  - [ ] Build prototype.
  - [ ] Generate QR code.
  - [ ] Test on Desktop.
  - [ ] Test on Movile.
     
- [ ] Solution 2:
  - [ ] Build prototype.
  - [ ] Generate QR code.
  - [ ] Test on Desktop.
  - [ ] Test on Movile.

### A/B Testing

N° Solution | Link             | Ease of use | Speed | Bugs                                 
----------- | ---------------- | ----------- | ----- | ------------------------------------   
1           | [Prototype 1](#) | ???         | ???   | ???                                 
2           | [Prototype 2](#) | ???         | ???   | ???                                 

