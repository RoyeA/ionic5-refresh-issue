# ionic5-refresh-issue

in your HTML template: 
---------------------
 <ion-refresher slot="fixed" (ionRefresh)="doRefresh($event)">
    <ion-refresher-content></ion-refresher-content>
  </ion-refresher>

in your ts code:
----------------
 doRefresh(event){
    event.target.complete();
  }



When pulling the screen once, the code run, and the refresher dissapear.
But since the first pull, the next one is (look like ) disabled.
