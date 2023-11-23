# pt-normalization

Portuguese speaking Python/C++ Developer for Portuguese NLP & Text Optimization project
Posted 4 days ago
Worldwide
We need a text normalization module that effectively processes Portuguese text, focusing on monetary values, special characters, punctuation, whitespace, capitalization, numerical expressions, and time formats.
We need to support both Locals, Brazil and Europe.

In more details:
Monetary Value Processing: The module must accurately identify and normalize Portuguese currency symbols and formats.

Special Characters and Punctuation: A system to interpret and normalize Portuguese punctuation and special characters, such as cedillas (ç), acute accents (á, é, í, ó, ú), and tildes (ã, õ), should be implemented.

Character Whitelisting: A whitelist for permissible characters will be utilized, specifically including Portuguese alphabets, numerals, and special characters. Non-whitelisted characters must be addressed by the system to ensure data integrity.

Whitespace Normalization: The software will consolidate multiple spaces into a single space to clean up text presentation.

Capitalization Management: The module will manage the capitalization of letters according to Portuguese language rules, such as the case sensitivity of proper nouns and the non-capitalization of days and months in regular text flow.

Edge Case and Error Resolution: Formulate methods to manage Portuguese-specific edge cases involving uncommon punctuation or syntax, and implement an error resolution process for accurate symbol replacements.

Numerical and Time Format Handling: The module must be capable of converting and formatting numerical values and time expressions to align with Portuguese conventions.

Hyphenated Word and Apostrophe Processing: Accurately process Portuguese hyphenated words and apostrophes in contractions and possessive forms.

Regression Testing: Implement regression testing to ensure the module's reliability, reflecting the ongoing changes and norms in the Portuguese language.

Unit Testing: Develop a comprehensive unit testing protocol to validate the functionality of individual components, promoting the system’s stability and maintainability.

Strategic Approaches for Portuguese Text Normalization:

Phased Processing Architecture: Embrace a phased processing approach, beginning with numerical and monetary normalization, followed by special character and punctuation management, and finalizing with capitalization adjustments.

Error Management Strategy: Adopt error prevention practices that avoid the need for error handling mechanisms by using rigorous input validation and clearly defined functions.

Comma Management Strategy: A context-based approach should be taken to manage commas, adding them according to Portuguese grammatical rules and textual context for precise normalization.
-------------------
See two quick examples:
See two examples:
Input1 - "A reunião começará às 14h30 na sala 3B - é importante que todos cheguem pontualmente."
Output1 - A reunião começará às quatorze horas e trinta minutos na sala três B , é importante que todos cheguem pontualmente.
Input2 - "Em 2023, o preço do livro era R$30,50; contudo, com o desconto de 5%, passou a ser R$28,97."
Output2 - Em dois mil e vinte e três, o preço do livro era trinta reais e cinquenta centavos; contudo, com o desconto de cinco por cento, passou a ser vinte e oito reais e noventa e sete centavos.


--------------------------------------------------------------------------------------
If you use Python, use standard and basic libraries, we need to convert it C++ later.

We will supply text files for testing and for development
