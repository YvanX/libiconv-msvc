How to compile libiconv:
1. Extract libiconv-x.xx.tar.gz to .\libiconv\libiconv
2. Edit .\libiconv\libiconv.rc. Set version to current version
3. Copy .\libiconv\libiconv\include\iconv.h.in to .\libiconv\iconv.h
4. Edit iconv.h and subsitution character '@' to empty.
5. Open Visual Studio to compile libiconv

Install:
Edit iconv.h with follow steps
subsitution DLL_VARIABLE to empty
subsitution line "#define EILSEQ EILSEQ" to "#define EILSEQ"
subsitution ICONV_CONST to empty
subsitution USE_MBSTATE_T to 1
subsitution BROKEN_WCHAR_H to 0
