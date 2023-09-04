# HPFinder (Dataset) for AsiaCCS 2024

This is the dataset introduced in our paper, "HPFinder: A Novel Approach to Automatically Analyze Android Malware with Obfuscated Anti-Sandbox Techniques".
The dataset consists of the following two datasets:

1. Obfuscated samples:
We collected the samples from Google Play and VirusTotal. We checked that it is working in our experiment board operating AOSP 10.
We obfuscated the samples with the control flow flattening and reflection. To apply control flow flattening, we used the BlackObfuscator, a open-source obfuscator for an Android app.
We also used the Obfuscapk to apply reflection. These two obfuscation techniques are well-known and widespread in the read-world.
The samples contained at least one anti-sandbox feature among root, tamper, and debugger detection.
We do not provide an APK file directly. It's because there might be a legal problem. So we provide MD5 hash value.

The file name contains the summary information about the anti-sandbox feature and experiment result in the HPFinder.
It's like this "Root-D-R".
"Root" means that the sample contains a root detection feature.
"D" means that HPFinder detected the root detection feature.
"R" means that HPFinder successfully removed the root detection feature.

As we explained in the paper, we found some interesting samples containing cross-language, multi-threaded anti-sandbox features.
The sample's hash values are the following.

-- MD5 hashes

* Multi-thread samples - 7

dc614310e63b38316e297bf89cc7d775

c446bb5e7d0def05906811c8fe682121

4b27a27f26547923647187c254be02c7

5614ca849f18cff234d0cb067442d5e3

e3d172673d6c1e7ab3cb2db971039a0e

c9b650486d9b3e512ac24f0822e0ddad

f6c372d9b9b21b2ba9e46c17ab9e7606


* Cross-language samples - 3

2e73af63489f60f9d033c4a38fd66990

a10452e68158fbe86115f9e0eea0d394

bb620c0111c59d5e8e1ef438f499f544


 * Mixed samples - 5
 
ff41bd6ed433c138fac937ab8bfa5e64

95642caa494bc4322ac2090ecdf3cf39

6b9395916e09bba99f554e682416a464

9f9f736af56e89a6be7bc6d7297d8f76

551791ae21f77732b28c9b1da3943dda



3. EBTSuite:
   






