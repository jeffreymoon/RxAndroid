# RxJava Releases #

### Version 0.25 - June 27th 2015 ###

* New: `RxAndroidPlugins` and its `RxAndroidSchedulersHook` provides a mechanism similar to `RxJavaPlugins` (and its `RxJavaSchedulersHook`) for
  changing the scheduler returned from `AndroidSchedulers.mainThread()` as well as a callback for each subscription on any `Handler`-based scheduler.
* Fix: Ensure errors are properly propagated from `ContentObservable.fromCursor`.
* Fix: `LifecycleObservable` now correctly unsubscribes from its sources.

Breaking changes:

* Users of `AppObservable.bindFragment` with a support-v4 `Fragment` should now use `bindSupportFragment`.


### Version 0.24 – January 3rd 2015 ###

This release has some breaking changes:

* `rx.android.observables.AndroidObservable` has changed to `rx.android.app.AppObservable`;
* `ViewObservable` has moved from `rx.android.observables` to `rx.android.view`
* (as part of RxJava's breaking changes) [`collect` has changed](https://github.com/ReactiveX/RxJava/blob/1a94d55fa8896931175896d09b86dca8d8d44f72/CHANGES.md#collect)


### Version 0.22 – October 15th 2014 ###

This release adds a number of new operators:

* [Pull 25](https://github.com/ReactiveX/RxAndroid/pull/25) Add operator to monitor SharedPreference changes
* [Pull 22](https://github.com/ReactiveX/RxAndroid/pull/22) Add view state event types to streamline ViewObservable
* [Pull 20](https://github.com/ReactiveX/RxAndroid/pull/20) Add OperatorAdapterViewOnItemClick to observe OnItemClick events in AdapterViews

### Version 0.21 – October 1st 2014 ###

Initial release outside the RxJava core project, no changes.
