# ion-app-contenteditable-ios

Steps to recreate:
1. ionic start ion-app-contenteditable-ios blank --capacitor
2. edit app.component.html
```
<div contenteditable="true" style="height: 100px; background: teal">Editable, outside ion-app</div>
<ion-app style="margin-top: 100px;">
  <div contenteditable="true" style="height: 100px; background: tomato">Editable, inside ion-app</div>
</ion-app>
```
3. ionic build
4. npx cap add ios
5. npx cap open ios

Test in simulator.
Can edit contenteditable within ion-app for android and web, but not ios.
