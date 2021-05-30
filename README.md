# DxMint Liquidity Generator

The following document will share details on how to verify code of your Liquidity Generator Token

### BSCScan, EtherScan or Similar
1. Start by first navigating to the verification section of BSCScan (https://bscscan.com/verifyContract) (Or for your chain)
2. Enter your DxMint generated token address 
3. For Compiler Type select "Solidity (Single File)"
4. For Compiler Version select "v0.6.12+commit.27d51765"
5. For Open Source License Type select "3) MIT License (MIT)"
6. Click continue
7. Now in the optimization field on the right select "Yes"
8. In the section that says enter solidity contract code below copy paste the contract for your chain from the chains folder in this github repository
9. At the very bottom of the page Verify the Captcha and click the Verify and Publish button
10. BSCScan will print an error saying "ByteCode (what we are looking for):"
    - Scroll all the way to the right of this section you will see a lot of 00000000000000's followed by a few numbers
    - Scroll to the left until the 0000000000000's stop 
    - You will see the following code {ipfs}64736f6c634300060c0033 at the end just before the long 00000000000000's start
    - Copy everything after the c0033 line (including the 00000's) 
    - [Sample copy: 000000000000000000000000f476cc43eeee4ad1d9f974ce1efffcafaf2a5e6a00000000000000000000000000000000000000000000000000000000000001400000000000000000000000000000000000000000000000000000000000000180000000000000000000000000000000000000000000000000000000000000001200000000000000000000000000000000000000000e8d9f193e6574c89800000000000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000003000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000003200000000000000000000000000000000000000000000000000000000000000074e45504a554e450000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000034e50450000000000000000000000000000000000000000000000000000000000]
11. Scroll down and click the start over button
12. In the section that says "Constructor Arguments ABI-Encoded" copy paste the variables copied from step 10 above
13. Verify the Captcha and click the Verify and Publish button.
14. Your code should now be verified.
