## Selenium TestNG Sandbox

A basic UI testing project to show basic usage of Selenium with TestNG as well as to experiment with different ways of performing automated UI testing (webdriver management, reporting, POM abstractions, etc).

## Quick Start

1. Ensure current JDK is installed (nothing else is required -- other dependencies will automatically download )
2. To run tests with Chrome run: ./gradlew
3. To tun tests with PhatomJS(Headless) run: ./gradlew testPhantomJs

## Notes

When running from Gradle -- the build script will automatically try to download required OS specific drivers for Chrome or PhatomJS, and update requirement environment variables -- phantomjs.binary.path or webdriver.chrome.driver

When running from an IDE -- you will need these environment variables setup and pointing to the correct webdriver

Example for running individual tests from the commandline: gradle testPhantomJs -Dtest.single=TestNgExample
