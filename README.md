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
