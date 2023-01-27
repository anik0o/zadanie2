# Zadanie nr 2 
## CZĘŚĆ NIEOBOWIĄZKOWA

CZĘŚĆ DRUGA

Pytanie: Czy istnieje mechanizm który mógłby całościowo zorganizować proces
kontroli nad tag-owaniem, a jeśli tak, to jak on
funkcjonuje ?

AWS posiada własną politykę i mechanizm tagowania obiektów.
Tagowanie jest nadaniem etykiety składającej się z klucza i wartości zdefiniowanej przez użytkownika.
Przykładowo poniższy tag składa się z klucza 'Stack ' i wartości 'production':

`aws ec2 create-tags \
    --resources ami-1234567890abcdef0 --tags Key=Stack,Value=production`

Tagi mogą pomóc w zarządzaniu, identyfikowaniu, organizowaniu, wyszukiwaniu i filtrowaniu zasobów.
Przykładowo tagi są bardzo często wykorzystywane przy uzyskiwaniu dostępu do danych zasobów, na przykład można określić, że użytkownik może uzyskać dostęp do zasobu, gdy zarówno użytkownik, jak i zasób mają tę samą wartość dla określonego tagu. 

Obiekty AWS można tagować pojedyńczo:

`aws ec2 create-tags \
    --resources ami-1234567890abcdef0 --tags Key=Stack,Value=production`
    
ale również zbiorowo: 

`aws ec2 create-tags \
    --resources ami-1a2b3c4d i-1234567890abcdef0 \
    --tags Key=webserver,Value=   Key=stack,Value=Production`

Wyróżniane są 4 kategorie tagów, ze względu na ich zastosowanie w zarządzaniu zasobami:

-Tagi techniczne 

-Tagi w celu automatyzacji 

-Tagi biznesowe 

-Tagi bezpieczeństwa


Wykorzystane linki:

https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html

https://aws.amazon.com/blogs/mt/implement-aws-resource-tagging-strategy-using-aws-tag-policies-and-service-control-policies-scps/
