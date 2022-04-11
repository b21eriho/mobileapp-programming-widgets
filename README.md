# Report

Created a textView inside the chosen Layout, constraintLayout.This textview was given a text to hold which wa also extracted into a string resource.
It was further given a text-size that was very large and was anchored to the top left, to give it the appearance of a title. It was given a small margin
and its size was set to wrap its content, it was also given an id.

After this an image was created, set to fill the screen width-wise and hold a set height. Its content was set to a medium grey color which was also
extracted to a color resource. It was set to lay beneath the title and given a small margin, it was also given an id. Due to its width being set to fill the 
entire screen it wasn't needed to constrain it horizontally.

Lastly a button was created and given a text to hold which was also extracted to a color resource. It's width was set statically while its height was set
to wrap its content. The size of the text was given in "sp" to have it resize according to user preference. Its top was constrained to the image's bottom
and both its sides were constrained to the image's sides. Resulting in it being centered horizontally. It was given a sizeable margin to set it apart from
the other views in the project. This might cause strange appearance if the text is set to be too large.

Below the source code for the button and a screenshot of the app are provided.

```
<Button
        android:id="@+id/button"
        android:layout_width="128dp"
        android:layout_height="wrap_content"
        android:text="@string/button_text"
        android:textSize="24sp"
        app:layout_constraintEnd_toEndOf="@+id/iamge"
        app:layout_constraintStart_toStartOf="@+id/iamge"
        app:layout_constraintTop_toBottomOf="@+id/iamge"
        android:layout_margin="64dp"/>
```

![](Screenshot.png)
