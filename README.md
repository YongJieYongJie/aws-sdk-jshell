# aws-sdk-jshell

Spin up a JShell with all of AWS SDK's classes a tab-completion away ✨

### Example usage:
  - Run `mvn jshell:run`
  - Copy-and-paste snippets from [AWS official code examples][code-examples] to
    explore the SDK
  - Profit?

### FAQs:
1. It is taking forever to load, is there some way to speed things up?
    - Start-up time can be reduced by not importing all the common AWS classes
      at start-up, by using the following command `mvn jshell:run -Dscripts=''`.
      However, this also means that tab-completion will not be available until
      the relevant classes are manually imported with the usual import
      statements.

[code-examples]: https://github.com/awsdocs/aws-doc-sdk-examples/tree/main/javav2/example_code
