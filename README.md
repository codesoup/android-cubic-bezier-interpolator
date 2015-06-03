**Deprecated**: use https://developer.android.com/reference/android/support/v4/view/animation/PathInterpolatorCompat.html instead.

android-cubic-bezier-interpolator
=================================

An Android Library that helps you implement bezier animations in you application

How to use
----------

```java
Animation animation = new Animation() {
    @Override
    protected void applyTransformation(float interpolatedTime, Transformation t) {
        super.applyTransformation(interpolatedTime, t);
        myView.setAlpha(interpolatedTime);
    }
};

//define the CubicBezierInterpolator
Interpolator easeInOut = new CubicBezierInterpolator(.1, .7, .1, 1);
animation.setInterpolator(easeInOut);

animation.setDuration(3000);
myView.startAnimation(animation);
```
