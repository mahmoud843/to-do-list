<div class="tab">
  <button class="tablinks" (click)="openTab('AngularList')">Angular List</button>
  <button class="tablinks" (click)="openTab('Playground')">Playground</button>
  <button class="tablinks" (click)="openTab('CodeWithCure')">CodeWithCure</button>
  <button class="tablinks" (click)="openTab('UnichatCourse')">Unichat Course</button>
</div>

<!-- Tab content -->
<div id="AngularList" class="tabcontent" *ngIf="currentTab === 'AngularList'">
  <h3>Angular List</h3>
  <p>Content for Angular List.</p>
</div>

<div id="Playground" class="tabcontent" *ngIf="currentTab === 'Playground'">
  <h3>Playground</h3>
  <p>Content for Playground.</p>
</div>

<div id="CodeWithCure" class="tabcontent" *ngIf="currentTab === 'CodeWithCure'">
  <h3>CodeWithCure</h3>
  <p>Content for CodeWithCure.</p>
</div>

<div id="UnichatCourse" class="tabcontent" *ngIf="currentTab === 'UnichatCourse'">
  <h3>Unichat Course</h3>
  <p>Content for Unichat Course.</p>
</div>
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  currentTab: string = 'AngularList';

  openTab(tabName: string) {
    this.currentTab = tabName;
  }
}
/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
}

/* Style the buttons inside the tab */
.tab button {
  background-color: inherit;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
  font-size: 17px;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}
