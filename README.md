Routing Using  Angular 2
Introduction: Angular  2 is a complete JavaScript-based open-source front-end web application framework mainly maintained by Google and by a community of individuals and corporations to address many of the challenges encountered in developing single-page applications.
Angular 2 is not a version upgrade, but a complete rewrite.
Routing in Angular is navigating from one view to another.
Steps:
1. Import RouterModule and Routes from angular/core library.  
2. Define the different paths in routes array as path and component pairs.
3. Pass the routes array in the forRoot function of RouterModule and declare it in the imports array of ngModule.
4. Export the respective components which are declared in the paths.

5. In app.component, inside component decorator create a template shown below.
6. In department-detail.component import ActivatedRoute

7. Use the snapshot function to fetch the id from the URL and display it on the screen.


Summary
The application has a configured router. The shell component has a RouterOutlet where it can display views produced by the router. It has RouterLinks that users can click to navigate via the router.
Here are the key Router terms and their meanings:
Router Part	Meaning
Router	Displays the application component for the active URL. Manages navigation from one component to the next.
RouterModule	A separate Angular module that provides the necessary service providers and directives for navigating through application views.
Routes	Defines an array of Routes, each mapping a URL path to a component.
Route	Defines how the router should navigate to a component based on a URL pattern. Most routes consist of a path and a component type.
RouterOutlet	The directive (<router-outlet>) that marks where the router should display a view.
RouterLink	The directive for binding a clickable HTML element to a route. Clicking an element with a routerLink directive that is bound to a string or a link parameters array triggers a navigation.
RouterLinkActive	The directive for adding/removing classes from an HTML element when an associated routerLink contained on or inside the element becomes active/inactive.
ActivatedRoute	A service that is provided to each route component that contains route specific information such as route parameters, static data, resolve data, global query params and the global fragment.
RouterState	The current state of the router including a tree of the currently activated routes together with convenience methods for traversing the route tree.
Link parameters array	An array that the router interprets as a routing instruction. You can bind that array to a RouterLink or pass the array as an argument to the Router.navigate method.
Routing component	An Angular component with a RouterOutlet that displays views based on router navigations.



