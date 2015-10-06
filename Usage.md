# Introduction #

This page will explain how to use the WSDLMerge tool.

You can find precompiled binaries in the Download section.

You can also [compiled](compile.md) it yourself.

# Details #

WSDLMerge is a command line utility (just like many other .NET tools). You need to open a command prompt to run it. You can also invoke it if you are using PowerShell, just like you would any other command line utility.

The tool requires either one or two parameters.

The first parameters is always the root WSDL document. If this is a local file, then this is all that is required.

For example:

```
> WSDLMerge.exe service.wsdl
```

If the root WSDL is a web address, you will need to specify a second parameter, which is a local filename. This file will be written as the output of the tool (the merged WSDL)

```
> WSDLMerge.exe http://localhost/test.svc?WSDL local.wsdl
```