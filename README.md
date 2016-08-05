# Android-XML-Animations

animations availible for use in your Android Studio projects.You places these XMl files inside of you **anim** folder which should be inside of your **res** folder

you can initialize animations as followed 
```
final Animation shrink = AnimationUtils.loadAnimation(context, R.anim.shrink);

shrink.setAnimationListener(new Animation.AnimationListener() {
    @Override
    public void onAnimationStart(Animation animation) {

    }

    @Override
    public void onAnimationEnd(Animation animation) {
        Intent info = new Intent(v.getContext(),webActivity.class);
        info.putExtra("site",dataPerson.get(position).getWebsite());
        v.getContext().startActivity(info);



    }

    @Override
    public void onAnimationRepeat(Animation animation) {

    }
});
Card.startAnimation(shrink);
```
