Retrofit Converters
===================
[![Build Status](https://travis-ci.org/ligboy/retrofit-converter-fastjson.svg?branch=master)](https://travis-ci.org/ligboy/retrofit-converter-fastjson)

Retrofit ships with support for OkHttp's `RequestBody` and `ResponseBody` types but the library is
content-format agnostic. The child modules contained herein are additional converters for other
popular formats.

To use, supply an instance of your desired converter when building your `Retrofit` instance.

```java
Retrofit retrofit = new Retrofit.Builder()
  .baseUrl("https://api.example.com")
  .addConverterFactory(FastJsonConverterFactory.create())
  .build();
```

#### Deploy
```bash
mvn deploy --settings settings
```
