## HELLO 🎉
resforx repository now opened!

resforx is BE & DBA programmer and made zetaform

> ## Zetaform
>> zetaform is JS library which find html elements using tag names and attributes
>>
>> zetaform is now beta version to prepare, and make it
>>
>> ## Usage
>> ### installation
>> you can use yarn or npm to install it
>> 
>> yarn:
>> ```yarn
>> yarn add zetaform
>> ```
>>
>> npm:
>> ```npm
>> npm install zetaform
>> ```
>>
>> ### statements
>>
>> htmlsector(): htmlsector is a method which find html elements with using tags or attributes
>> ```javascript
>> const htmlsector = (tag, attribute, html) => {
>>    const regex = new RegExp(`<${tag} ${attribute}.*?>([\\s\\S]*?)<\/${tag}>`, 'g');
>>    let match = regex.exec(html);
>>    const result = [];
>>    const content = [];
>>    while (match != null) {
>>        result.push(match[0]); 
>>        content.push(match[1]);  
>>        match = regex.exec(html);
>>    }
>>    return {
>>        value: () => content.join(' '), 
>>        toString: () => result.join(' ')
>>    };
>>}
>> ```
>>
>> to use htmlsector,
>> ```javascript
>> htmlsector("tag (like h1, p)", "attribute (like class, id)", <variable name>);
>> ```
>>
>> variable name is which you write parameters in fs function, fs will be need because fs module helps reading html files

## Contact
#### for more contact of resforx, come to <feather076@gmail.com> or <paedeogim@gmail.com>
