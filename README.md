"# AndroidDialog" 


<p>

<center>
    <bold>
AndroidDialog support: Text Mode, Image Mode, Text & Image Mode
PromptDialog support: Success, Info, Error, Warning, Help
Support custom in/out animation
With many Features.
    </bold>


allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
}
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>






dependencies {
   implementation 'com.github.sandeep7788:AndroidDialog:1.0.0'
}

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>






Simple Java Code for Android
<br>

<code>

ColorDialog dialog = new ColorDialog(this);
<br>
dialog.setTitle(getString(R.string.operation));
<br>
dialog.setContentText(getString(R.string.content_text));
<br>
dialog.setContentImage(getResources().getDrawable(R.mipmap.sample_img));
<br>
dialog.setPositiveListener(getString(R.string.delete), new ColorDialog.OnPositiveListener() {
<br>
    @Override
    <br>
    public void onClick(ColorDialog dialog) {
    <br>
        Toast.makeText(MainActivity.this, dialog.getPositiveText().toString(), Toast.LENGTH_SHORT).show();
        <br>
    }
    <br>
})
<br>
.setNegativeListener(getString(R.string.cancel), new ColorDialog.OnNegativeListener() {
<br>
    @Override
    <br>
    public void onClick(ColorDialog dialog) {
    <br>
        Toast.makeText(MainActivity.this, dialog.getNegativeText().toString(), Toast.LENGTH_SHORT).show();
        <br>
        dialog.dismiss();
        <br>
    }
    <br>
}).show();
<br>
</code>
</center>
</p>
<br>
<br>
<br>
<br>
<br>
