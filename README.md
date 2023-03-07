# @royalf1sh/vue-phone-mask

[![Version](https://img.shields.io/npm/v/vue-phone-mask-input.svg)](https://www.npmjs.com/package/vue-phone-mask)
[![License](https://img.shields.io/npm/l/vue-phone-mask-input.svg)](https://www.npmjs.com/package/vue-phone-mask)
[![Monthly Downloads](https://img.shields.io/npm/dm/vue-phone-mask-input.svg)](https://www.npmjs.com/package/vue-phone-mask)

![example 1](https://i.ibb.co/6JzBsYD/example1.gif)


## Installation

### npm
```
npm i vue-phone-mask --save
```


## Usage
```javascript
import PhoneMaskInput from  "vue-phone-mask";
```
```html
<template>
    <div>
      <h2>Example 4 [custom style]</h2>
      <phone-mask-input
        v-model="phone"
        autoDetectCountry
        showFlag
        @onValidate="onValidate"
        wrapperClass="wrraper-example"
        inputClass="input-example"
        flagClass="flag-example"
      />
      <p>
        Phone number:
        <b>{{phone}}</b>
      </p>
      <p class="json">{{valid}}</p>
    </div>
</template>
```
![example 2](https://i.ibb.co/YZ2dgDL/example2.gif)


## Props
| Name | Type | Default | Description |
| --- | --- | ---| --- |
| value | [String, Number] |  | Value to be render in the input |
| placeholder | String | "" | Placeholder to be shown when no tags | 
| autoDetectCountry | Boolean | false | Detect visitor country |
| defaultCountry | String |  | one of the values defined [here](#available-flags) |
| showFlag | Boolean | false | Show country flag |
| flagSize | String | normal | Available values: small, normal, big |
| disabled | Boolean | false | Disable input field |
|  wrapperClass | String | { display: flex; flex-direction: row; align-items: center; height: 40px; }| Style class of div wrapper input and flag|
| inputClass | String | { height: 20px; }| Style class of input|
| flagClass | String | { margin: 0; } |  Style class of flag (span tag) |


## Events
| Property value | Arguments| Description |
| --- | --- | ---|
| input | String | Fires when the input changes with the argument is the string number |
| isValid | Object | Fires when the input changes with the argument is the object includes { number, isValid, country } |
| onBlur | | Fires on blur event |
| onFocus | | Fires on focus event |


## Available Flags

Here follows the list of the available flags. They are identified using the [ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1) standard.  
This component currently support **alpha-2** of the standard.  

| **Country Name** | **alpha-2** |
|--------------|------|
| Afghanistan  | af | 
| Aland Islands  | ax | 
| Albania  | al | 
| Algeria  | dz |
| American Samoa  | as |
| Andorra  | ad |
| Angola  | ao |
| Anguilla  | ai |
| Antigua and Barbuda  | ag |
| Argentina  | ar |
| Armenia  | am |
| Aruba  | aw 
| Australia  | au |
| Austria  | at |
| Azerbaijan  | az |
| Bahamas  | bs |
| Bahrain  | bh |
| Bangladesh  | bd |
| Barbados  | bb |
| Belarus  | by |
| Belgium  | be |
| Belize  | bz |
| Benin  | bj |
| Bermuda  | bm |
| Bhutan  | bt |
| Bolivia  | bo |
| Bosnia and Herzegovina  | ba |
| Botswana  | bw |
| Brazil  | br |
| British Virgin Islands  | vg |
| Brunei  | bn |
| Bulgaria  | bg |
| Burkina Faso  | bf |
| Burma  | mm |
| Burundi  | bi |
| Cambodia  | kh |
| Cameroon  | cm |
| Canada  | ca |
| Canary Islands | ic |
| Cape Verde  | cv |
| Cayman Islands  | ky |
| Central African Republic  | cf |
| Chad  | td | 
| Chile  | cl |
| China  | cn |
| Colombia  | co |
| Comoros  | km |
| Cook Islands  | ck |
| Costa Rica  | cr |
| Croatia  | hr |
| Cuba  | cu |
| Curacao | cw |
| Cyprus  | cy | 
| Czech Republic  | cz |
| Democratic Republic of the Congo  | cd | 
| Denmark  | dk |
| Djibouti  | dj | 
| Dominica  | dm |
| Dominican Republic  | do |
| East Timor  | tl |
| Ecuador  | ec |
| Egypt  | eg |
| El Salvador  | sv | 
| Equatorial Guinea  | gq | 
| Eritrea  | er | 
| Estonia  | ee | 
| Ethiopia  | et | 
| European Union | eu |
| Falkland Islands (Malvinas)  | fk |
| Faroe Islands  | fo |
| Fiji  | fj |
| Finland  | fi |
| France  | fr |
| French Polynesia  | pf |
| French Southern Territories  | tf |
| Gabon  | ga |
| Gambia  | gm | 
| Georgia  | ge |
| Germany  | de | 
| Ghana  | gh | 
| Gibraltar  | gi |
| Granada  | gd |
| Greece  | gr | 
| Greenland  | gl |
| Guam  | gu | 
| Guatemala  | gt | 
| Guernsey  | gg | 
| Guinea  | gn | 
| Guinea-Bissau  | gw |
| Guyana  | gy | 
| Haiti  | ht | 
| Honduras  | hn | 
| Hong Kong  | hk | 
| Hungary  | hu | 
| Iceland  | is | 
| India  | in | 
| Indonesia  | id | 
| Iran  | ir |
| Iraq  | iq | 
| Ireland  | ie |
| Isle of Man  | im | 
| Israel  | il | 
| Italy  | it | 
| Ivory Coast  | ci | 
| Jamaica  | jm | 
| Japan  | jp | 
| Jersey  | je | 
| Jordan  | jo | 
| Kazakhstan  | kz | 
| Kenya  | ke | 
| Kiribati  | ki | 
| Kuwait  | kw |
| Kyrgyzstan  | kg |
| Laos  | la | 
| Latvia  | lv | 
| Lebanon  | lb | 
| Lesotho  | ls |
| Liberia  | lr | 
| Libya  | ly | 
| Liechtenstein  | li | 
| Lithuania  | lt | 
| Luxembourg  | lu |
| Macao  | mo | mac |
| Macedonia  | mk | 
| Madagascar  | mg | 
| Malawi  | mw |
| Malaysia  | my | 
| Maldives  | mv | 
| Mali  | ml | mli |
| Malta  | mt |
| Marshall, Islands  | mh | 
| Martinique  | mq | 
| Mauricio  | mu | 
| Mauritania  | mr |
| Mayotte  | yt | 
| Mexico  | mx | 
| Micronesia  | fm |
| Moldova  | md |
| Monaco  | mc | 
| Mongolia  | mn | 
| Montenegro  | me | 
| Montserrat  | ms |
| Morocco  | ma | mar |
| Mozambique  | mz | moz |
| Namibia  | na | nam |
| Nauru  | nr | nru |
| Nepal  | np | npl |
| Netherlands Antilles  | an | 
| New Caledonia  | nc | 
| New Zealand  | nz |
| Nicaragua  | ni | 
| Niger  | ne | 
| Nigeria  | ng |
| Niue  | nu | 
| Norfolk, Island  | nf |
| North Korea  | kp | 
| Northern Mariana Islands  | mp | 
| Norway  | no |
| Oman  | om | 
| Pakistan  | pk | 
| Palau  | pw | 
| Palestine  | ps | 
| Panama  | pa | 
| Papua New Guinea  | pg |
| Paraguay  | py | pry |
| Peru  | pe | per |
| Philippines  | ph | 
| Pitcairn  | pn | 
| Poland  | pl | 
| Portugal  | pt | 
| Puerto Rico  | pr | 
| Qatar  | qa | 
| Republic of the Congo  | cg | 
| Romania  | ro | 
| Russia  | ru | 
| Rwanda  | rw | 
| Saint Barthelemy  | bl | 
| Saint Helena  | sh | 
| Saint Kitts and Nevis  | kn | 
| Saint Lucia  | lc | 
| Saint Martin  | mf | 
| Saint Vincent and the Grenadines  | vc |
| Samoa  | ws | 
| San Marino  | sm | 
| Sao Tome and Principe  | st | 
| Saudi Arabia  | sa | 
| Senegal  | sn | 
| Serbia  | rs | 
| Seychelles  | sc | 
| Sierra Leone  | sl | 
| Singapore  | sg | 
| Slovakia  | sk | 
| Slovenia  | si | 
| Solomon Islands  | sb | 
| Somalia  | so | 
| South Africa  | za | 
| South Georgia and the South Sandwich Islands  | gs | 
| South Korea  | kr | 
| South Sudan  | ss | 
| Spain  | es | 
| Sri Lanka  | lk | 
| Sudan  | sd | 
| Suriname  | sr | 
| Swaziland  | sz | 
| Sweden  | se | 
| Switzerland  | ch | 
| Syria  | sy | 
| Taiwan  | tw | 
| Tajikistan  | tj | 
| Tanzania  | tz | 
| Thailand  | th | 
| The Netherlands  | nl | 
| Togo  | tg | 
| Tokelau  | tk | 
| Tonga  | to | 
| Trinidad and Tobago  | tt | 
| Tunisia  | tn | 
| Turkey  | tr | 
| Turkmenistan  | tm | 
| Turks and Caicos Islands  | tc | 
| Tuvalu  | tv | 
| Uganda  | ug | 
| Ukraine  | ua | 
| United Arab Emirates  | ae | 
| United Kingdom  | gb | 
| United States  | us | 
| Uruguay  | uy | 
| Uzbekistan  | uz | 
| Vanuatu  | vu | 
| Vatican City  | va | 
| Venezuela  | ve | 
| Vietnam  | vn | 
| Virgin Islands of the United States  | vi | 
| Wallis and Futuna  | wf |
| Western Sahara  | eh |
| Yemen  | ye |
| Zambia  | zm | 
| Zimbabwe  | zw | 


