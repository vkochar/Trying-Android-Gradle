FakeLibraryProductFlavors
=========================

The source contains two flavors in the Lib > pro, free

To use the lib with the pro code/resources included use

    gradlew preparePro assemble

and to use the lib with free code/resources included use

    gradlew prepareFree assemble


The ***build.gradle*** under Lib contains tasks created to prepare for pro/free version.
Those tasks being

    preparePro
    prepareFree
    
They essentially copy and replace whatever is inside ***src/main*** before the actuall build/assemble takes place.



###NOTE
This is not merging of code or resources, but in fact just replacing with the appropriate flavor.

Whatever that does not need to be replaced can stay under ***src/main***.

