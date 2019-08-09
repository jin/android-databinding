```
$ bazel build :app_prod
2019/08/09 17:43:25 Using unreleased version at commit c082f02ba2d07a97363596ed087c83e29a4582ed
INFO: Analyzed target //:app_prod (3 packages loaded, 347 targets configured).
INFO: Found 1 target...
ERROR: /Users/jingwen/code/android-databinding/BasicSample/BUILD.bazel:4:1: Linking static android resource library for //:lib_prod_base failed (Exit 1) ResourceProcessorBusyBox failed: error executing command bazel-out/host/bin/external/bazel_tools/src/tools/android/java/com/google/devtools/build/android/ResourceProcessorBusyBox --tool LINK_STATIC_LIBRARY -- --aapt2 ... (remaining 17 argument(s) skipped)

Use --sandbox_debug to see verbose messages from the sandbox
Aug 09, 2019 5:43:35 PM com.google.devtools.build.android.AndroidManifest parseFrom
WARNING:
CONFIGURATION: bazel-out/android-armeabi-v7a-fastbuild/bin/lib_prod_base_processed_manifest/AndroidManifest.xml has no minSdkVersion. Using 1.
Aug 09, 2019 5:43:37 PM com.google.devtools.build.android.ValidateAndLinkResourcesAction main
SEVERE: Error while validating and linking resources
java.lang.RuntimeException: Error during Statically linking com.google.devtools.build.android.aapt2.CompiledResources@4802796d:
Command: bazel-out/host/bin/external/androidsdk/aapt2_binary\
	link\
	--static-lib\
	--manifest\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/manifest-aapt-dummy/AndroidManifest.xml\
	--no-static-lib-packages\
	--no-version-vectors\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_appcompat_appcompat_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_interpolator_interpolator_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_fragment_fragment_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_viewmodel_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_localbroadcastmanager_localbroadcastmanager_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_legacy_legacy_support_core_utils_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_core_core_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_versionedparcelable_versionedparcelable_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_livedata_core_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_arch_core_core_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_print_print_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_livedata_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_documentfile_documentfile_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_loader_loader_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_slidingpanelayout_slidingpanelayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_customview_customview_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_cursoradapter_cursoradapter_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_coordinatorlayout_coordinatorlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_viewpager_viewpager_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_asynclayoutinflater_asynclayoutinflater_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_legacy_legacy_support_core_ui_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_swiperefreshlayout_swiperefreshlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_drawerlayout_drawerlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_vectordrawable_vectordrawable_animated_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_vectordrawable_vectordrawable_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_constraintlayout_constraintlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_extensions_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_service_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_process_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_databinding_databinding_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_databinding_databinding_adapters_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/lib_prod_base_symbols/symbols.zip\
	-I\
	external/androidsdk/platforms/android-28/android.jar\
	--auto-add-overlay\
	-o\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/lib.apk\
	--java\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/java\
	--output-text-symbols\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/R.txt
Output:
app/src/main/res/layout/observable_field_profile.xml:68: error: '@{user.likes < 4 ? R.drawable.ic_person_black_96dp : R.drawable.ic_whatshot_black_96dp }' is incompatible with attribute srcCompat (attr) reference [weak].
app/src/main/res/layout/observable_field_profile.xml:68: error: '@{user.likes > 9 ? @color/star : @android:color/black}' is incompatible with attribute tint (attr) color.
app/src/main/res/layout/observable_field_profile.xml:155: error: attribute progressScaled (aka com.example.android.databinding.basicsample:progressScaled) not found.
app/src/main/res/layout/observable_field_profile.xml:155: error: '@{100}' is incompatible with attribute max (attr) integer.
app/src/main/res/layout/observable_field_profile.xml:155: error: '@{ConverterUtil.isZero(user.likes)}' is incompatible with attribute visibility (attr) enum [gone=2, invisible=1, visible=0].
app/src/main/res/layout/viewmodel_profile.xml:65: error: attribute popularityIcon (aka com.example.android.databinding.basicsample:popularityIcon) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute hideIfZero (aka com.example.android.databinding.basicsample:hideIfZero) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute progressScaled (aka com.example.android.databinding.basicsample:progressScaled) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute progressTint (aka com.example.android.databinding.basicsample:progressTint) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: '@{100}' is incompatible with attribute max (attr) integer.
error: failed linking file resources.

	at com.google.devtools.build.android.AaptCommandBuilder.execute(AaptCommandBuilder.java:318)
	at com.google.devtools.build.android.aapt2.ResourceLinker.linkStatically(ResourceLinker.java:273)
	at com.google.devtools.build.android.ValidateAndLinkResourcesAction.main(ValidateAndLinkResourcesAction.java:195)
	at com.google.devtools.build.android.ResourceProcessorBusyBox$Tool$12.call(ResourceProcessorBusyBox.java:132)
	at com.google.devtools.build.android.ResourceProcessorBusyBox.processRequest(ResourceProcessorBusyBox.java:237)
	at com.google.devtools.build.android.ResourceProcessorBusyBox.main(ResourceProcessorBusyBox.java:198)

Aug 09, 2019 5:43:37 PM com.google.devtools.build.android.ResourceProcessorBusyBox processRequest
SEVERE: Error during processing
java.lang.RuntimeException: Error during Statically linking com.google.devtools.build.android.aapt2.CompiledResources@4802796d:
Command: bazel-out/host/bin/external/androidsdk/aapt2_binary\
	link\
	--static-lib\
	--manifest\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/manifest-aapt-dummy/AndroidManifest.xml\
	--no-static-lib-packages\
	--no-version-vectors\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_appcompat_appcompat_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_interpolator_interpolator_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_fragment_fragment_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_viewmodel_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_localbroadcastmanager_localbroadcastmanager_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_legacy_legacy_support_core_utils_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_core_core_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_versionedparcelable_versionedparcelable_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_livedata_core_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_arch_core_core_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_print_print_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_livedata_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_documentfile_documentfile_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_loader_loader_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_slidingpanelayout_slidingpanelayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_customview_customview_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_cursoradapter_cursoradapter_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_coordinatorlayout_coordinatorlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_viewpager_viewpager_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_asynclayoutinflater_asynclayoutinflater_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_legacy_legacy_support_core_ui_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_swiperefreshlayout_swiperefreshlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_drawerlayout_drawerlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_vectordrawable_vectordrawable_animated_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_vectordrawable_vectordrawable_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_constraintlayout_constraintlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_extensions_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_service_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_process_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_databinding_databinding_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_databinding_databinding_adapters_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/lib_prod_base_symbols/symbols.zip\
	-I\
	external/androidsdk/platforms/android-28/android.jar\
	--auto-add-overlay\
	-o\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/lib.apk\
	--java\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/java\
	--output-text-symbols\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/R.txt
Output:
app/src/main/res/layout/observable_field_profile.xml:68: error: '@{user.likes < 4 ? R.drawable.ic_person_black_96dp : R.drawable.ic_whatshot_black_96dp }' is incompatible with attribute srcCompat (attr) reference [weak].
app/src/main/res/layout/observable_field_profile.xml:68: error: '@{user.likes > 9 ? @color/star : @android:color/black}' is incompatible with attribute tint (attr) color.
app/src/main/res/layout/observable_field_profile.xml:155: error: attribute progressScaled (aka com.example.android.databinding.basicsample:progressScaled) not found.
app/src/main/res/layout/observable_field_profile.xml:155: error: '@{100}' is incompatible with attribute max (attr) integer.
app/src/main/res/layout/observable_field_profile.xml:155: error: '@{ConverterUtil.isZero(user.likes)}' is incompatible with attribute visibility (attr) enum [gone=2, invisible=1, visible=0].
app/src/main/res/layout/viewmodel_profile.xml:65: error: attribute popularityIcon (aka com.example.android.databinding.basicsample:popularityIcon) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute hideIfZero (aka com.example.android.databinding.basicsample:hideIfZero) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute progressScaled (aka com.example.android.databinding.basicsample:progressScaled) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute progressTint (aka com.example.android.databinding.basicsample:progressTint) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: '@{100}' is incompatible with attribute max (attr) integer.
error: failed linking file resources.

	at com.google.devtools.build.android.AaptCommandBuilder.execute(AaptCommandBuilder.java:318)
	at com.google.devtools.build.android.aapt2.ResourceLinker.linkStatically(ResourceLinker.java:273)
	at com.google.devtools.build.android.ValidateAndLinkResourcesAction.main(ValidateAndLinkResourcesAction.java:195)
	at com.google.devtools.build.android.ResourceProcessorBusyBox$Tool$12.call(ResourceProcessorBusyBox.java:132)
	at com.google.devtools.build.android.ResourceProcessorBusyBox.processRequest(ResourceProcessorBusyBox.java:237)
	at com.google.devtools.build.android.ResourceProcessorBusyBox.main(ResourceProcessorBusyBox.java:198)

Exception in thread "main" java.lang.RuntimeException: Error during Statically linking com.google.devtools.build.android.aapt2.CompiledResources@4802796d:
Command: bazel-out/host/bin/external/androidsdk/aapt2_binary\
	link\
	--static-lib\
	--manifest\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/manifest-aapt-dummy/AndroidManifest.xml\
	--no-static-lib-packages\
	--no-version-vectors\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_appcompat_appcompat_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_interpolator_interpolator_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_fragment_fragment_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_viewmodel_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_localbroadcastmanager_localbroadcastmanager_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_legacy_legacy_support_core_utils_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_core_core_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_versionedparcelable_versionedparcelable_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_livedata_core_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_arch_core_core_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_print_print_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_livedata_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_documentfile_documentfile_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_loader_loader_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_slidingpanelayout_slidingpanelayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_customview_customview_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_cursoradapter_cursoradapter_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_coordinatorlayout_coordinatorlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_viewpager_viewpager_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_asynclayoutinflater_asynclayoutinflater_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_legacy_legacy_support_core_ui_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_swiperefreshlayout_swiperefreshlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_drawerlayout_drawerlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_vectordrawable_vectordrawable_animated_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_vectordrawable_vectordrawable_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_constraintlayout_constraintlayout_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_extensions_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_service_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_lifecycle_lifecycle_process_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_databinding_databinding_runtime_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/external/maven/androidx_databinding_databinding_adapters_symbols/symbols.zip\
	-R\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/filtered/bazel-out/android-armeabi-v7a-fastbuild/bin/lib_prod_base_symbols/symbols.zip\
	-I\
	external/androidsdk/platforms/android-28/android.jar\
	--auto-add-overlay\
	-o\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/lib.apk\
	--java\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/java\
	--output-text-symbols\
	/var/folders/6s/dh8ytxkd39l2k3jmpqgxzjvr00ch_3/T/android_resources_tmp5532907378362982445/R.txt
Output:
app/src/main/res/layout/observable_field_profile.xml:68: error: '@{user.likes < 4 ? R.drawable.ic_person_black_96dp : R.drawable.ic_whatshot_black_96dp }' is incompatible with attribute srcCompat (attr) reference [weak].
app/src/main/res/layout/observable_field_profile.xml:68: error: '@{user.likes > 9 ? @color/star : @android:color/black}' is incompatible with attribute tint (attr) color.
app/src/main/res/layout/observable_field_profile.xml:155: error: attribute progressScaled (aka com.example.android.databinding.basicsample:progressScaled) not found.
app/src/main/res/layout/observable_field_profile.xml:155: error: '@{100}' is incompatible with attribute max (attr) integer.
app/src/main/res/layout/observable_field_profile.xml:155: error: '@{ConverterUtil.isZero(user.likes)}' is incompatible with attribute visibility (attr) enum [gone=2, invisible=1, visible=0].
app/src/main/res/layout/viewmodel_profile.xml:65: error: attribute popularityIcon (aka com.example.android.databinding.basicsample:popularityIcon) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute hideIfZero (aka com.example.android.databinding.basicsample:hideIfZero) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute progressScaled (aka com.example.android.databinding.basicsample:progressScaled) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: attribute progressTint (aka com.example.android.databinding.basicsample:progressTint) not found.
app/src/main/res/layout/viewmodel_profile.xml:147: error: '@{100}' is incompatible with attribute max (attr) integer.
error: failed linking file resources.

	at com.google.devtools.build.android.AaptCommandBuilder.execute(AaptCommandBuilder.java:318)
	at com.google.devtools.build.android.aapt2.ResourceLinker.linkStatically(ResourceLinker.java:273)
	at com.google.devtools.build.android.ValidateAndLinkResourcesAction.main(ValidateAndLinkResourcesAction.java:195)
	at com.google.devtools.build.android.ResourceProcessorBusyBox$Tool$12.call(ResourceProcessorBusyBox.java:132)
	at com.google.devtools.build.android.ResourceProcessorBusyBox.processRequest(ResourceProcessorBusyBox.java:237)
	at com.google.devtools.build.android.ResourceProcessorBusyBox.main(ResourceProcessorBusyBox.java:198)
Target //:app_prod failed to build
Use --verbose_failures to see the command lines of failed build steps.
INFO: Elapsed time: 11.870s, Critical Path: 3.00s
INFO: 25 processes: 25 darwin-sandbox.
FAILED: Build did NOT complete successfully
```


Android Data Binding Basic Sample
=============================================

This sample showcases the following features of the
[Data Binding library](https://developer.android.com/topic/libraries/data-binding/index.html):

* Layout variables and expressions
* Observability through Observable Fields, LiveData and Observable classes
* Binding Adapters, Binding Methods and Binding Converters
* Seamless integration with ViewModels

It shows common bad practices and their solutions in two different screens.

Features
--------

![Screenshot](https://github.com/googlesamples/android-databinding/blob/master/BasicSample/screenshots/screenshotbasic.png)

### Layout variables and expressions

With Data Binding you can write less boilerplate and repetitive code. It moves UI operations out
of the activities and fragments to the XML layout.

For example, instead of setting text on a TextView in an activity:

```java
TextView textView = findViewById(R.id.name);
textView.setText(user.name);
```

You assign the attribute to a variable, in the XML layout:

```xml
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="@{user.name}" />
```

See `ObservableFieldActivity.kt`, `ObservableFieldProfile.kt` and `observable_field_profile.xml`
for a simple example.

### Observability

In order to update the UI automatically when the data changes, Data Binding lets you bind attributes
with observable objects. You can choose between three mechanisms to achieve this: Observable fields,
LiveData and Observable classes.

#### Observable fields

Types like ObservableBoolean, ObservableInt and the generic ObservableField replace the
corresponding primitives to make them observable. Setting a new value on one of the Observable
fields will update the layout automatically.

```kotlin
class ProfileObservableFieldsViewModel : ViewModel() {

    val likes = ObservableInt(0)

    fun onLike() {
        likes.increment()  // Equivalent to set(likes.get() + 1)
    }
}
```

In this example, when `onLike` is called, the number of likes is incremented
and the UI is updated. There is no need to notify that the property changed.

#### LiveData

LiveData is an observable from
[Android Architecture Components](https://developer.android.com/topic/libraries/architecture)
that is lifecycle-aware. 

The advantages over Observable Fields are that LiveData supports
[Transformations](https://developer.android.com/reference/android/arch/lifecycle/Transformations)
and it's compatible with other components and libraries, like Room and WorkManager.

```kotlin
class ProfileLiveDataViewModel : ViewModel() {
    private val _likes =  MutableLiveData(0)
    val likes: LiveData<Int> = _likes // Expose an immutable LiveData

    fun onLike() {
        _likes.value = (_likes.value ?: 0) + 1
    }
}
```

It requires an extra step done on the binding:


```kotlin

binding.lifecycleOwner = this  // use viewLifecycleOwner when assigning a fragment
```

#### Observable classes

For maximum flexibility and control, you can implement a fully observable class and decide when
to update certain properties. This lets you create dependencies between properties and it's
useful to dispatch partial UI updates, for example avoiding
potential glitches (UI elements updating almost at the same time).

```kotlin
class ProfileObservableViewModel : ObservableViewModel() {
    val likes = ObservableInt(0)

    fun onLike() {
        likes.increment()
        notifyPropertyChanged(BR.popularity)
    }

    @Bindable
    fun getPopularity(): Popularity {
        return likes.get().let {
            when {
                it > 9 -> Popularity.STAR
                it > 4 -> Popularity.POPULAR
                else -> Popularity.NORMAL
            }
        }
    }
}
```

In this example, when `onLike` is called, the number of likes is incremented and the
`popularity` property is notified of a potential change (`popularity` depends on `likes`).
`getPopularity` is called by the library, returning a possible new value.

See `ProfileObservableFieldsViewModel.kt` for a complete example.

#### Binding adapters

Binding adapters let you customize or create layout attributes. For example, you can create
an `app:progressTint` attribute for progress bars where you change the color of the
progress indicator depending on an external value.

```kotlin
    @BindingAdapter("app:progressTint")
    @JvmStatic fun tintPopularity(view: ProgressBar, popularity: Popularity) {

        val color = getAssociatedColor(popularity, view.context)
        view.progressTintList = ColorStateList.valueOf(color)
    }
```

The binding is created in the XML layout with:

```xml
    <ProgressBar
        app:progressTint="@{viewmodel.popularity}" />
```

Using binding adapters lets you move UI calls from the activity to static methods, improving
encapsulation.

You can also use multiple attributes in a Binding Adapter, see `viewmodel_profile.xml` for a complete
example.

#### Binding methods and binding converters

Binding methods and binding converters let you reduce code if your binding adapters
are very simple. You can read about them in the
[official guide](https://developer.android.com/topic/libraries/data-binding/index.html#attribute_setters).

For example, if an attribute's value needs to be passed to a method in the class:

```kotlin
@BindingAdapter("app:srcCompat")
@JvmStatic fun srcCompat(view: ImageView, @DrawableRes drawableId: Int) {
    view.setImageResource(drawable)
}
```

You can replace this with a Binding Method which can be added to any class in the project:

```kotlin
@BindingMethods(
        BindingMethod(type = ImageView::class,
                attribute = "app:srcCompat",
                method = "setImageDrawable"))
```

#### Binding Converters (use with caution)

In this sample we show a View depending on whether a number is zero. There are many options to do
this. We're showing two, one in the `observable_field_profile.xml`
and, the recommended way, in `viewmodel_profile.xml`.

The goal is to bind the view's visibility to the number of likes, but this won't work:

```xml
android:visibility="@{viewmodel.likes}"  <!-- Doesn't work as expected -->
```

The number of likes is an integer and the visibility attribute takes an integer
(`VISIBLE`, `GONE` and `INVISIBLE` are 0, 4 and 8 respectively), so doing this would build,
but the result would not be the expected.

A possible solution is:

```xml
android:visibility="@{viewmodel.likes == 0 ? View.GONE : View.VISIBLE}"/
```

But it adds a relatively complex expression to the layout.

Instead, you can create and import a utils class:

```xml
<data>
        <import type="com.example.android.databinding.basicsample.util.ConverterUtil" />
        ...
</data>
```

and use it from the View like so:

```xml
android:visibility="@{ConverterUtil.isZero(viewmodel.likes)}"  <!-- don't do this either -->
```

`isZero` returns a boolean and `visibility` takes an integer so in order to convert
from boolean we can also define a BindingConversion:

```kotlin
    @BindingConversion
    @JvmStatic fun booleanToVisibility(isVisible: Boolean): Int {  // Risky! applies everywhere
        return if (isVisible) View.VISIBLE else View.GONE
    }
```

This conversion is unsafe because this binding conversion is not restricted to our case: it will
convert all booleans to visibility integers when the attribute takes an integer.

Solution: As with every BindingConversion and BindingMethod, you can replace it with a Binding
Adapter, which normally is much simpler:

```kotlin
    @BindingAdapter("app:hideIfZero")  // Recommended solution
    @JvmStatic fun hideIfZero(view: View, number: Int) {
        view.visibility = if (number == 0) View.GONE else View.VISIBLE
    }
```

and as shown in in `viewmodel_profile.xml`:

```xml
app:hideIfZero="@{viewmodel.likes}"
```

This defines a new custom attribute `hideIfZero` that can't be used accidentally.

As a rule of thumb it's preferable to create your our custom attributes using Data Binding adapters
instead of adding logic to your binding expressions.

Sample app
----------

This app shows a user's profile using two different screens to showcase different Data Binding
features:

  * Main activity: Shows how a Data Binding layout lets you access Views without `findViewById`.

  * Observable field activity: In this screen the user can give "likes" to the profile and the UI
  reacts automatically to changes. However, the activity  holds the logic that receives the user
  click and the actual profile data, which is not testable.
  Also, likes are reset when the user rotates the device and the layout contains documented common
  bad practices.

  * ViewModel activity: Using a ViewModel from the
  [Architecture Components](https://developer.android.com/topic/libraries/architecture/index.html)
  fixes the rotation problem and moves logic out of the activity. Also, the use of binding
  adapters changes the responsibility of the activity which is no longer the "view" and
  solely responsible for dealing with the lifecycle. Two ViewModels are suggested in
  `ProfileObservableViewModel.kt`: one based on observable fields and another implementing the
  observable interface.


License
--------

Copyright 2018 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.
