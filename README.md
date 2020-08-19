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



AndroidDialog dialog = new AndroidDialog(this);
        dialog.setTitle(getString(R.string.operation));
        dialog.setContentText(getString(R.string.content_text));
        dialog.setContentImage(getResources().getDrawable(R.mipmap.sample_img));
        dialog.setPositiveListener(getString(R.string.delete), new AndroidDialog.OnPositiveListener() {
            @Override
            public void onClick(AndroidDialog dialog) {
                Toast.makeText(MainActivity.this, dialog.getPositiveText().toString(), Toast.LENGTH_SHORT).show();
            }
        }).setNegativeListener(getString(R.string.cancel), new AndroidDialog.OnNegativeListener() {
                    @Override
                    public void onClick(AndroidDialog dialog) {
                        Toast.makeText(MainActivity.this, dialog.getNegativeText().toString(), Toast.LENGTH_SHORT).show();
                        dialog.dismiss();
                    }
                }).show();
<br>

</center>
</p>
<br>
<br>
<br>
<br>
