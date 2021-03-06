# Easy-Readable-Speakable-Codes
Unambiguous code generation for unique ID codes that need to be relayed in some way, either read or spoken without similar sounding or looking characters. I.E. No O and 0 (Zero)

Simple? Yes. But then, why does nobody seem to do it?

```Console.WriteLine(EasyCodes.Generator.GetCode());```  

OUTPUT: PXVKJQ
  
  
```Console.WriteLine(EasyCodes.Generator.GetCode(10));```  

OUTPUT: 27JGPQZUCA
    
  
```Console.WriteLine(EasyCodes.Generator.GetCode(8, CharacterSets.LettersOnly));```  

OUTPUT: PLGUAUPV


## Also with SplitCodes() method to make codes more easily readable:  

```  
var TestCodeTwo = "GXHYDHWTTQPYRY4QWQLCFKLH7G";
        
var result = Generator.SplitCode(TestCodeTwo);
result.Should().Be("GXHY DHWT TQPY RY4Q WQLC FKLH 7G");

var result = Generator.SplitCode(TestCodeTwo,3,"-");
result.Should().Be("GXH-YDH-WTT-QPY-RY4-QWQ-LCF-KLH-7G");
```
