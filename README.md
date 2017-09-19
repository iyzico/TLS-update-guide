# TLS  v1.2 Requirement

The Payment Card Industry Security Standards Council (PCI SSC) [mandates](https://blog.pcisecuritystandards.org/migrating-from-ssl-and-early-tls) that all credit card processors must retire early versions of TLS from service by the PCI deadline.

As part of this requirement, iyzico is making this upgrade and updating all services to require TLS 1.2 for all HTTPS connections.


# Update Guide for Iyzico Merchants

## Python

Python 2.6 will not be supported in March 2018 for TLS 1.2 migration. Please upgrade your Python version to minimum 2.7.9. Latest [iyzipay-python](https://github.com/iyzico/iyzipay-python)  library required after python update.

## Ruby

Ruby 1.9.3 will not be supported in March 2018 for TLS 1.2 migration. Please upgrade your Ruby version to minimum 2.0.0. Latest [iyzipay-ruby](https://github.com/iyzico/iyzipay-ruby)  library required after ruby update.

## Java

### Java 1.8

No change is required and Java 1.8 is preferred for iyzico because TLS v1.2 is the default in Java 1.8.

### Java 1.7

Latest [iyzipay-java](https://github.com/iyzico/iyzipay-java) library required. No code change is required.

### Java 1.6

TLS v1.2 is not officially supported for public Oracle JDK 6 releases but Oracle JDK update 121 paid-for release should be used. Latest [iyzipay-java](https://github.com/iyzico/iyzipay-java) library required. Iyzico prefers upgrading to Java 1.7 or Java 1.8.

### Java 1.5

TLS v1.2 is not supported.

## .NET

Latest [iyzipay-dotnet](https://github.com/iyzico/iyzipay-dotnet) library required. 

# Testing

You can use https://sandbox-api-tls12.iyzipay.com/ as base url for testing TLS 1.2 update.

# Support

If you have any questions, please open an issue on Github or contact us at integration@iyzico.com.



