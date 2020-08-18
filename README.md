"# AndroidDialog" 


<code>

AndroidDialog support: Text Mode, Image Mode, Text & Image Mode
PromptDialog support: Success, Info, Error, Warning, Help
Support custom in/out animation
With many Features.



allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
}







dependencies {
   implementation 'com.github.sandeep7788:AndroidDialog:1.0.0'
}








Simple Java Code for Android




ColorDialog dialog = new ColorDialog(this);
dialog.setTitle(getString(R.string.operation));
dialog.setContentText(getString(R.string.content_text));
dialog.setContentImage(getResources().getDrawable(R.mipmap.sample_img));
dialog.setPositiveListener(getString(R.string.delete), new ColorDialog.OnPositiveListener() {
    @Override
    public void onClick(ColorDialog dialog) {
        Toast.makeText(MainActivity.this, dialog.getPositiveText().toString(), Toast.LENGTH_SHORT).show();
    }
})
.setNegativeListener(getString(R.string.cancel), new ColorDialog.OnNegativeListener() {
    @Override
    public void onClick(ColorDialog dialog) {
        Toast.makeText(MainActivity.this, dialog.getNegativeText().toString(), Toast.LENGTH_SHORT).show();
        dialog.dismiss();
    }
}).show();
</code>
