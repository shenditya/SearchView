# SearchView

Next version 3.0 will be released in April or May 2016 with changes and fixes.

If you want to be prepared for next release then test version 
# 0.1.4 
is uploaded to jCenter. 
It has some new features, but be aware that version has a lot of changes and still has bugs !!! Otherwise use version 2.2 (below this text).

------------------------------------------------------------------------------------------------------------------------------

Because I have done firstly this library as a private project, 
I would like to know if someone of you use my library in your application. 
If yes, please send me a name of your app and link to Play Store and I will promote your app in Readme.

------------------------------------------------------------------------------------------------------------------------------

Persistent SearchView Library like Play Store. 

Check sample project very thoroughly !!!

Features: Material Design, Toolbar / Menu item version, History, Styling.

Google Material Design Pattern:
https://www.google.com/design/spec/patterns/search.html

Version history here:
https://bintray.com/lapism/maven/searchview/view

Material colors in the project:
https://gist.github.com/lapism/3b417142300d9dbde3b4

Sample application on:

<a href="https://play.google.com/store/apps/details?id=com.lapism.searchview.sample">
  <img alt="Get it on Google Play"
       src="https://github.com/lapism/SearchView/blob/master/images/google_play.png" />
</a>

# Usage
**Add the dependencies to your gradle file:**
```javascript
dependencies {
        compile 'com.lapism:searchview:2.2'
        }
```

![Screenshot 1]
(https://github.com/lapism/SearchView/blob/master/images/image_1.png)![Screenshot2]
(https://github.com/lapism/SearchView/blob/master/images/image_2.png)![Screenshot 3]
(https://github.com/lapism/SearchView/blob/master/images/image_3.png)![Screenshot 4]
(https://github.com/lapism/SearchView/blob/master/images/image_4.png)![Screenshot 5]
(https://github.com/lapism/SearchView/blob/master/images/image_5.png)![Screenshot 6]
(https://github.com/lapism/SearchView/blob/master/images/image_6.png)

**Code:**
```java
    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        switch (item.getItemId()) {
            case R.id.action_search: {
                mSearchView.show(true/false); // animate, ONLY FOR MENU ITEM
                return true;
            }
            default:
                return super.onOptionsItemSelected(item);
        }
    }
```

**XML:**
```xml
<com.lapism.searchview.view.SearchView
    android:id="@+id/searchView"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
```

**Styling SearchView:**
```
app:search_version = "toolbar / menu_item"
app:search_style = "toolbar_classic / menu_item_classic / menu_item_color"
app:search_theme = "light / dark"
app:search_divider = "true / false"
app:search_hint = "Hint text"
app:search_hint_size = "16sp"
app:search_voice = "true / false"
app:search_voice_text = "Voice text"
app:search_animation_duration = "360"
app:search_shadow_color = "#80000000"
```

**Apps using this library:**

[Service Notes](https://play.google.com/store/apps/details?id=notes.service.com.servicenotes)
