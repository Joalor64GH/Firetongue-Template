# Firetoungue Template

Just a quick template for you guys to use if your games have language localization.

Through the provided folders, images, audio, and text can all be translated.
When your game is built, the translations from here will be pulled into your game.

## Adding a new language

Follow these steps to add a new language:
1. Create a new language folder with the correct locale code for your language.
	- The locale code is based on the language as well as the region you wish to translate for. For example, Braziliian Portuguese is pt-BR.
	- As an example of regions, American English is `en-US`, where as British English is `en-GB`.
2. Add the corresponding entries to the `index.xml` file.
	- You will need to add a new `<locale>` tag, which will provide a list of contributors.
	- You will also need to provide translations for basic UI elements needed for the user interface, such as the "Okay" button.
	- You will also need to go to the other languages and provide a translation for the name of your language. For example, the `Portuguese` language needs to contain the Portuguese words for `French`, `English`, etc.
3. Add the translations to the locale's folder.
	- Be sure to translate text and, if able, images and audio assets.

### Replacement characters

Some special characters will cause translation to break. Use Firetongue's special replacement characters to deal with these situations:

```
<Q>  = Standard single quotation mark ( " )
<LQ> = Fancy left quotation mark ( “ )
<RQ> = Fancy right quotation mark ( ” )
<C>  = Standard comma
<N>  = Line break
<T>  = Tab
<RE>[$SOME_FLAG] = Replace with the value of the flag
```

## Last Things

Credits go to [EliteMasterEric](https://github.com/EliteMasterEric) for the [original repository](https://github.com/EnigmaEngine/EnigmaTranslation).

Also, contibutions would be nice :))