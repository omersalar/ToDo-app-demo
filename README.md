# Pre-work - *SimplyDo*

**SimplyDo** is an android app that allows building a todo list and basic todo items management functionality including adding new items, editing and deleting an existing item.

Submitted by: **Syed Omer Khureshi**

Time spent: **10** hours spent in total

## User Stories

The following **required** functionality is completed:

* [X] User can **successfully add and remove items** from the todo list
* [X] User can **tap a todo item in the list and bring up an edit screen for the todo item** and then have any changes to the text reflected in the todo list.
* [X] User can **persist todo items** and retrieve them properly on app restart

The following **optional** features are implemented:

* [ ] Persist the todo items [into SQLite](http://guides.codepath.com/android/Persisting-Data-to-the-Device#sqlite) instead of a text file
* [ ] Improve style of the todo items in the list [using a custom adapter](http://guides.codepath.com/android/Using-an-ArrayAdapter-with-ListView)
* [ ] Add support for completion due dates for todo items (and display within listview item)
* [ ] Use a [DialogFragment](http://guides.codepath.com/android/Using-DialogFragment) instead of new Activity for editing items
* [ ] Add support for selecting the priority of each todo item (and display in listview item)
* [ ] Tweak the style improving the UI / UX, play with colors, images or backgrounds

The following **additional** features are implemented:

* [ ] List anything else that you can get done to improve the app functionality!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

<img src='http://i.imgur.com/ZdwbuEc.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with [Peek](https://github.com/phw/peek#peek---an-animated-gif-recorder).

## Project Analysis

As part of your pre-work submission, please reflect on the app and answer the following questions below:

**Question 1:** "What are your reactions to the Android app development platform so far? Compare and contrast Android's approach to layouts and user interfaces in past platforms you've used."

**Answer:** I have had previous experience building simple Android apps and I feel it's not difficult to get started learning Android app development. However, there is a huge list of concepts that are a developer must understand to build slightly complex apps. But there are very good resources on internet, including the CodePath cliffnotes and the official Android documentation, to learn new APIs and understand their usage.

I have previously used JavaFX and feel it is very similar to the Android layouting framework, in that both provide an XML based layouting that can be augmented dynamically with java. This enables a cleaner seperation of views from logic.

**Question 2:** "Take a moment to reflect on the `ArrayAdapter` used in your pre-work. How would you describe an adapter in this context and what is its function in Android? Why do you think the adapter is important? Explain the purpose of the `convertView` in the `getView` method of the `ArrayAdapter`."

**Answer:** As per documentation, when using a list based UI element backed by a collection, the `ArrayAdapter` provides objects that will populate each element in the list. By default the `toString` method is invoked on each element of the collection object and populated as a `TextView` on the UI. 

The `ArrayAdapter` invokes the `getView` method to obtain a view to display. If required, the view can be customized by overriding the `getView` method to return the custom view as desired. 

In order to improve performace and memory, the `ArrayAdapter` can reuse older views that are no longer displayed on the screen. The `convertView` parameter of the `getView` method receives the older views using which the `ArrayAdapter` can recycle them. If needed or in case the old view cannot be reused, the `getView` method can create new view as well.

The developers at StackOverflow have warned not to store state data in view as they may be reused and instead store the data in adapters.

## Notes

Describe any challenges encountered while building the app.

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.



