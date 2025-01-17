---
{
  "title": "Card (Token)",
  "schema": "card",
  "meta": [
    {
      "name": "description",
      "content": "Card (Token) data model documentation.",
    },
    {
      "property": "og:description",
      "content": "Card (Token) data model documentation."
    },
    {
      "name": "keywords",
      "content": "mtg, magic: the gathering, mtgjson, json, tokens, token, card (token)",
    }
  ],
  "feed": {
    "enable": "true"
  }
}
---

# Card (Token)

The Card (Token) data model describes the properties and values of a single card token.

**Parent model:** [Set](/file-models/set/)  
**Parent property:** `tokens`

## Model Index

<PropertyToggler/>

[[toc]]

## Model Properties

> ### artist  
> The name of the artist that illustrated the card art.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### asciiName  
> The [ASCII](http://www.asciitable.com) (Basic/128) code formatted card name with no special unicode characters.  
>
> - **Type:** `string`  
> - **Introduced:** `v5.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### availability  
> A list of the card's available printing types.  
>
> - **Type:** `array[string]`
> - <ExampleField type='availability'/>
> - **Introduced:** `v5.0.0`

> ### borderColor  
> The color of the card border.  
>
> - **Type:** `string`
> - <ExampleField type='borderColor'/>
> - **Introduced:** `v4.0.0`

> ### colorIdentity  
> A list of all the colors found in `manaCost`, `colorIndicator`, and `text`.  
>
> - **Type:** `array[] | array[string]`
> - <ExampleField type='colorIdentity'/>
> - **Introduced:** `v4.0.0`

> ### colorIndicator  
> A list of all the colors in the color indicator (The symbol prefixed to a card's [types](#types)).  
>
> - **Type:** `array[string]`
> - <ExampleField type='colorIndicator'/>
> - **Introduced:** `v4.0.2`
> - **Attributes:** <i class="optional">optional</i>

> ### colors  
> A list of all the colors in `manaCost` and `colorIndicator`. Some cards may not have a value, such as cards with `"Devoid"` in its `text`.  
>
> - **Type:** `array[] | array[string]`
> - <ExampleField type='colors'/>
> - **Introduced:** `v4.0.0`

> ### edhrecRank  
> The card rank on [EDHRec](https://www.edhrec.com).  
>
> - **Type:** `integer`  
> - **Introduced:** `v4.5.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### faceName  
> The name on the face of the card.  
>
> - **Type:** `string`  
> - **Introduced:** `v5.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### flavorText  
> The italicized text found below the rules text that has no game function.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### frameEffects  
> The visual frame effect.  
>
> - **Type:** `array[] | array[string]`
> - <ExampleField type='frameEffects'/>
> - **Introduced:** `v4.6.0`

> ### frameVersion  
> The version of the card frame style.  
>
> - **Type:** `string`
> - <ExampleField type='frameVersion'/>
> - **Introduced:** `v4.0.0`

> ### hasFoil  
> If the card be found in foil.  
>
> - **Type:** `boolean`  
> - **Introduced:** `v4.0.0`

> ### hasNonFoil  
> If the card can be found in non-foil  
>
> - **Type:** `boolean`  
> - **Introduced:** `v4.0.0`

> ### identifiers  
> A list of identifiers associated to a card. See the [Identifiers](/data-models/identifiers/) data model.  
>
> - **Type:** `object{props}`  
> - **Introduced:** `v5.0.0`

> ### isFullArt  
> If the card has full artwork.  
>
> - **Type:** `boolean`  
> - **Introduced:** `v4.4.2`  
> - **Attributes:** <i class="optional">optional</i>  

> ### isOnlineOnly  
> If the card is only available in [Magic: The Gathering Online](https://magic.wizards.com/en/mtgo).  
>
> - **Type:** `boolean`  
> - **Introduced:** `v4.0.1`  
> - **Attributes:** <i class="optional">optional</i>  

> ### isPromo  
> If the card is promotional.  
>
> - **Type:** `boolean`  
> - **Introduced:** `v4.4.2`  
> - **Attributes:** <i class="optional">optional</i>  

> ### isReprint  
> If the card has been reprinted.  
>
> - **Type:** `boolean`  
> - **Introduced:** `v4.4.2`  
> - **Attributes:** <i class="optional">optional</i>  

> ### keywords  
> A list of keywords found on the card.  
>
> - **Type:** `array[string]`  
> - **Introduced:** `v5.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### layout  
> The type of card layout. For a token card, this will be `"token"`.  
>
> - **Type:** `string`
> - <ExampleField type='layout'/>
> - **Introduced:** `v4.0.0`

> ### loyalty  
> The loyalty value of the card. Used on Planeswalker cards. 
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### name  
> The name of the card. Cards with multiple faces, like `"Split"` and `"Meld"` cards are given a delimiter.
>
> - **Type:** `string`
> - **Example:** `"Wear // Tear"`
> - **Introduced:** `v4.0.0`

> ### number  
> The number of the card. Can be prefixed or suffixed with a `*` or other characters for promo sets.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`

> ### power  
> The power of the card.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### promoTypes  
> A list of promotional types for a card.  
>
> - **Type:** `array[string]`
> - <ExampleField type='promoTypes'/>
> - **Introduced:** `v5.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### reverseRelated
> The names of the cards that produce this card.  
>
> - **Type:** `array[string]`  
> - **Introduced:** `v4.0.0`

> ### setCode  
> The set code of the card.  
>
> - **Type:** `string`  
> - **Introduced:** `v5.0.1`

> ### side  
> The identifier of the card side. Used on cards with multiple faces.  
>
> - **Type:** `string`
> - <ExampleField type='side'/>
> - **Introduced:** `v4.1.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### subtypes  
> A list of card subtypes found after em-dash.  
>
> - **Type:** `array[] | array[string]`
> - <ExampleField type='subtypes'/>
> - **Introduced:** `v4.0.0`

> ### supertypes  
> A list of card supertypes found before em-dash.  
>
> - **Type:** `array[] | array[string]`
> - <ExampleField type='supertypes'/>
> - **Introduced:** `v4.0.0`

> ### text  
> The rules text of the card.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### toughness  
> The toughness of the card.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>  

> ### type  
> The type of the card as visible, including any supertypes and subtypes.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`

> ### types  
> A list of all card types of the card, including Un&#8209;sets and gameplay variants.
>
> - **Type:** `array[string]`
> - <ExampleField type='types'/>
> - **Introduced:** `v4.0.0`

> ### uuid  
> The universal unique identifier (v5) generated by MTGJSON. Each entry is unique.  
>
> - **Type:** `string`  
> - **Introduced:** `v4.0.0`

> ### watermark  
> The name of the watermark on the card.  
>
> - **Type:** `string`
> - <ExampleField type='watermark'/>
> - **Introduced:** `v4.0.0`  
> - **Attributes:** <i class="optional">optional</i>
