# Android Studio

1.
_Device as developer_
* Developer mode
* Media sync
* Run

2.
_Github_
* VCS -> Git
* Automatically created Git repository in default folder
* VCS -> Import into version control -> Github

Use terminal if there is git config problem

3.
_Images_
app/src/main/res/drawable-hdpi

4.
_Languages_
values-es
strings.xml with spanish values
activity_main -> Default language to Spanish

5.
_Button Click_
```java

final TextView firstTextView = (TextView) findViewById(R.id.textView);
  
Button firstButton = (Button) findViewById(R.id.button);
  
firstButton.setOnClickListener(new View.OnClickListener() {
  @Override
  public void onClick(View view) {
    firstTextView.setText("You Clicked");
  }
});
```