# GradientTextViewWithCustomAngle
![alt text](https://github.com/Dat-PV-134/GradientTextViewWithCustomAngle/blob/main/preview.jpg)

## Implementation:
Project setting gradle:

```sh
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven (url = "https://jitpack.io")
    }
}
```

Build.gradle (Module app):

```sh
  implementation("com.github.Dat-PV-134:GradientTextViewWithCustomAngle:1.0.0")
```

## Usage:

Set angle in xml

```sh
  <com.focus_and_simplicity.gradienttextviewwithcustomangle.GradientTextView
        android:id="@+id/tvHello"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textStyle="bold"
        android:textSize="36sp"
        app:angle="45"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
```

In code

```sh
  binding.tvHello.setListColor(listOf("#9b5fe0", "#16a4d8", "#60dbe8", "#8bd346", "#efdf48", "#f9a52c", "#d64e12"))
```
