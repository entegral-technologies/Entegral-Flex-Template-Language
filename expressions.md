# Flex Expressions #
Expressions allows you to define data placeholders and is simply placed anywhere in your HTML code. To get idea of the expressions you can read the Handlebars docs.

## Listings ##
Provides all the listings for this office. Listings can be filtered, sorted and limited.


### Iterate over a listings list ###
`{{#each listings}} ... {{/each}}`

`{{{#each listings}}} ... {{{/each}}}`
`{{{{#each listings}}}} ... {{{/{each}}}}`


Inner expression variables: You can use the individual listing expressions within a listing block.

### Listing expressions ###

{{propertyid}} : unique property id, e.g. 102001
{{streetaddress}} : the street address if property address revealed by user, e.g. 12 Main Road
{{complexname}} : the name of the complex, if revealed by user, e.g. Bastille
{{suburb}} :  the name of the suburb, e.g. Bryanston  
{{town}} : town of the property listing , e.g. Sandton
{{province}} : province name of the listing, e.g. Gauteng
{{propertyMaintype}} : main type of property, e.g. Residential
{{propertyType}} : type of property, e.g. House
{{propertyStatus}} : status of the listing, e.g. For Sale
{{currency}} : currency for the {{price}}, e.g. USD
{{price}} : property asking price, formatted, e.g. 4,500,000
{{mainphoto}} : main photo url
{{bedrooms}} : number of bedrooms, e.g. 3
{{bathrooms}} : number of bathsrooms, e.g. 2
{{garages}} : number of garages, e.g. 2
{{pool}} : if there is a pool, e.g. true
{{study}} : number of studies on property, e.g. 1 // new field to be confirmed
{{livingareas}} : number of living areas on property, e.g. 2 // new field to be confirmed
{{heading}} : short property heading for advertising purposes
{{description}} : long description for advertising purposes
{{suburb_longitude}} : suburb longitude e.g. 28.034088  
{{suburb_latitude}} : suburb latitude e.g.  ‎-26.195246
{{longitude}} : property longitude if supplied by user, e.g. 28.034088  
{{latitude}} : suburb latitude if supplied by user e.g.  ‎-26.195246
{{hasvideo}} : whether the property has a video, e.g Y
{{isonshow}} : whether the property is on show in future, e.g. N
{{ispricedrop}} : if the property price was dropped, e.g. N
{{isjustlisted}} : if the property was added in 4 weeks range
{{buildingsize}} : size of the land, e.g. 540sqm
{{standsize}} : size of the building, e.g. 230sqm
{{mandatetype}} : type of mandate, e.g. sole
{{showonmap}} : indicating whether user wants to show exact location of listing on map, 1=Yes, 2=No
{{staffquarters}} : indicate the number of staff quarters
{{ratestaxes}} : indicate the rates and taxes amount
{{carports}} : indicate the number of carports
{{levy}} : indicates the levy
{{photos.n}} : photo url of listing where n indicates which photo to display, so {{photos.0}} will display the main photo.  e.g.  http://img.entegral.net/p/n913199_cd17a0f3-2b4f-47a0-8d06-de8f387648b41.jpg 
Offices
Provides a list of offices linked to the website. Offices can be filtered, sorted and limited.



Iterate over an offices list

{{#each offices}} ... {{/each}}
Inner expression: You can use the individual office expressions within a office block.



Office expressions

{{office_name}} : name of the agency, e.g. ABC Real Estate
{{office_tel}} : telephone number of agency, e.g. 012-201-6777
{{office_fax}} : fax number of agency, e.g. 012-222-3333
{{office_email}} :  email address of office, e.g. info@entegral.net  
{{office_profile}} :  profile description of the office, e.g. We are the #1 estate agency in the Northern ...  
{{office_postaladdress}} :  postal address of agency, e.g. PO BOX 1282, Lonehill, 2062
{{office_logo}} :  the url of the agency logo
Agents
Provides a list of all agents for this office. Agents can be filtered, sorted and limited.



Iterate over an agents list

{{#each agents}} ... {{/each}}
Inner expressions: You can use the individual agent expressions within an agent block.



Agent expressions

{{agent_name}} : name of agent, e.g. John 
{{agent_lastname}} : last name of agent, e.g. Doe
{{agent_role}} : role of the agent, e.g. estate agent
{{agent_cell}} : mobile number of agebt , e.g. 082-222-3333
{{agent_email}} :  email address of agent, e.g. john@entegral.net  
{{agent_profile}} :  profile description of the agent, e.g. I am a specialist in residential rentals in...
{{agent_photo}} :  url of the agent photo
{{agent_officetel}} : telephone number of office of the agent, e.g. 012-201-6777
{{agent_links_privyseal}} : privyseal handle if supplied
{{agent_links_facebookl}} : facebook handle if supplied
{{agent_links_twitter}} : twitter handle if supplied
{{agent_links_linkedin}} : linkedin handle if supplied
{{agent_links_instagram}} : instagram handle if supplied
{{agent_links_skype}} : skype handle if supplied
Facets Suburb
Iterate over an facets list

{{#each facets_suburb}} ... {{/each}}
Inner expressions: You can use the individual facet expressions within a facet block.



Facet suburb expressions

{{count}} : count of properties within a suburb, e.g. 42 
{{suburb}} : suburb name, e.g. BAKOVEN
{{town}} : town name, e.g. CAPE TOWN
{{province}} : province name, e.g. WESTERN CAPE
Facets Town
Iterate over an facets list

{{#each facets_town}} ... {{/each}}
Inner expressions: You can use the individual facet expressions within a facet block.



Facet town expressions

{{count}} : count of properties within a town, e.g. 42 
{{town}} : town name, e.g. CAPE TOWN
{{province}} : province name, e.g. WESTERN CAPE
Facets Province
Iterate over an facets list

{{#each facets_province}} ... {{/each}}
Inner expressions: You can use the individual facet expressions within a facet block.



Facet province expressions

{{count}} : count of properties within a town, e.g. 42 
{{province}} : province name, e.g. WESTERN CAPE
Facets Property Main Type
Iterate over an facets list

{{#each facets_propertyMaintype}} ... {{/each}}
Inner expressions: You can use the individual facet expressions within a facet block.



Facet property main type expressions

{{count}} : count of properties with this main type, e.g. 42 
{{propertyMaintype}} : main type, e.g. Residential
Facets Property Type
Iterate over an facets list

{{#each facets_propertyType}} ... {{/each}}
Inner expressions: You can use the individual facet expressions within a facet block.



Facet property type expressions

{{count}} : count of properties with this type, e.g. 42 
{{propertyType}} : type, e.g. Apartment
Facets Property Status
Iterate over an facets list

{{#each facets_propertyStatus}} ... {{/each}}
Inner expressions: You can use the individual facet expressions within a facet block.



Facet property status expressions

{{count}} : count of properties with this status, e.g. 42 
{{propertyStatus}} : status, e.g. For Sale
Website
Object with your website settings

Usage

{{website.domain}}


Available fields

{{website.domain}}
{{website.bucketname}}
{{website.clientofficeid}}
{{website.sourceid}}
{{website.country}}
{{website.country_code}}
{{website.map_api_key}}
{{website.url_format_agent}}
{{website.url_format_property}}
{{website.url_format_province}}
{{website.url_format_suburb}}
{{website.url_format_town}}
{{website.url_format_office}}
Special variables
There are extra variables that available depending on template. 

property.html - property with the same expressions as listings entry;

suburb.html - suburb with the same expressions as facets suburb entry;

town.html - town with the same expressions as facets town entry;

province.html - province with the same expressions as facets entry;

agent.html - agent with the same expressions as agent entry.

office.html - office with the same expressions as office entry.
