# Run the project

---
### Requirements

- Have JDK 11 installed

### Run tests
```
./gradlew test --info
```

### Examine output
Running the tests with the above command should yield the following output:
```
AppTest > testFoo() FAILED
    java.lang.VerifyError: Expecting a stackmap frame at branch target 15
    Exception Details:
      Location:
        com/amazon/device/iap/model/RequestId.equals(Ljava/lang/Object;)Z @1: ifnull
      Reason:
        Expected stackmap frame at this location.
      Bytecode:
        0000000: 2bc6 000e 2ab6 0016 2bb6 0016 a500 0503
        0000010: ac2a b400 0e2b c000 06b4 000e b600 17ac
        0000020:
        at org.example.AppTest.testFoo(AppTest.java:12)
```