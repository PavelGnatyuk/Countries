# Countries
A demo project Search in Country list created in Xcode 9 beta 2 with iOS 11 SDK. 
The navigation bar has large title and contains the search controller - two UI additions from the WWDC 2017.
The following line sets large title for the current view controller and all controller followed after this
```swift
self.navigationController?.navigationBar.prefersLargeTitles = true
```
until the mode of the title is changed:
```swift
self.navigationController?.navigationItem.largeTitleDisplayMode = .never
```
The following code adds a search controller to the navigation bar:
```swift
let search = UISearchController(searchResultsController: nil)
search.searchResultsUpdater = self
self.navigationItem.searchController = search
```
