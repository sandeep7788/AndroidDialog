"# AndroidDialog" 


<p>

<center>
    <bold>
AndroidDialog support: Text Mode, Image Mode, Text & Image Mode
PromptDialog support: Success, Info, Error, Warning, Help
Support custom in/out animation
With many Features.
    </bold>


<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

allprojects {<br>
    repositories {<br>
        ...<br>
        maven { url "https://jitpack.io" }<br>
    }<br>
}<br>
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






Simple Java Code for Android <br>



        
AndroidDialog dialog = new AndroidDialog(this);
        <br>
        dialog.setTitle(getString(R.string.operation));
        <br>
        dialog.setContentText(getString(R.string.content_text));
        <br>
        dialog.setContentImage(getResources().getDrawable(R.mipmap.sample_img));
        <br>
        dialog.setPositiveListener(getString(R.string.delete), new AndroidDialog.OnPositiveListener() {
        <br>
            @Override]
        <br>
            public void onClick(AndroidDialog dialog) {
        <br>
                Toast.makeText(MainActivity.this, dialog.getPositiveText().toString(), Toast.LENGTH_SHORT).show();
        <br>
            }
        <br>
        }).setNegativeListener(getString(R.string.cancel), new AndroidDialog.OnNegativeListener() {
        <br>
                    @Override
        <br>
                    public void onClick(AndroidDialog dialog) {
        <br>
                        Toast.makeText(MainActivity.this, dialog.getNegativeText().toString(), Toast.LENGTH_SHORT).show();
        <br>
                        dialog.dismiss();
        <br>
                    }
        <br>
                }).show();
        <br>
 
<br>
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






Simple kotlin Code for android

<br>
val dialog = AndroidDialog(this)<br>
        dialog.setTitle(getString(R.string.operation))<br>
        dialog.contentText = getString(R.string.content_text)<br>
        dialog.setContentImage(resources.getDrawable(R.mipmap.sample_img))<br>
        dialog.setPositiveListener(<br>
            getString(R.string.delete)<br>
        ) { dialog -><br>
            Toast.makeText(<br>
                this@MainActivity,<br>
                dialog.positiveText.toString(),<br>
                Toast.LENGTH_SHORT<br>
            ).show()<br>
        }.setNegativeListener(<br>
            getString(R.string.cancel)<br>
        ) { dialog -><br>
            Toast.makeText(<br>
                this@MainActivity,<br>
                dialog.negativeText.toString(),<br>
                Toast.LENGTH_SHORT<br>
            ).show()<br>
            dialog.dismiss()<br>
        }.show()<br>

</center>
</p>
<br>
<br>
<br>
<br>
