# Product Manager API

# About ProductAttributes and CategoryAttributes
  • You can set category attributes as string with this format => attr1;attr2;attr3;attr4 <br />
  • You can set product attribute values as string with this format => val1;val2;val3;val4 <br />
  • AddProductToCategory() will set productAttributes like this => attr1=val1;attr2=val2;attr3=val3;attr4=val4; <br />
  • GetProductsByAttr(attr_name,attr_value) returns a list of products with attribute and value match <br />

# Example Category
  • CategoryTshirt <br />
  { <br />
    id=3, <br />
    name="Tshirts", <br />
    categoryAttributes="Size;Color;Gender;Brand" <br />
  } <br />

# Example Product
  • ProductTshirt <br />
  { <br />
    id=0, <br />
    name="Midnite Sky", <br />
    catalogId=3, <br />
    price=75, <br />
    productAttributes="XL;Black;Unisex;7artdesign" <br />
  } <br />
  
  # Example usage of GetProductsByAttr()
    • GetProductsByAttr("brand","7artdesign") <br />
