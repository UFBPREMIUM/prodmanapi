# Product Manager API

# About ProductAttributes and CategoryAttributes
  • You can set category attributes as string with this format => attr1;attr2;attr3;attr4\n
  • You can set product attribute values as string with this format => val1;val2;val3;val4
  • AddProductToCategory() will set productAttributes like this => attr1=val1;attr2=val2;attr3=val3;attr4=val4;
  • GetProductsByAttr(attr_name,attr_value) returns a list of products with attribute and value match

# Example Category
  • CategoryTshirt
  {
    id=3,
    name="Tshirts",
    categoryAttributes="Size;Color;Gender;Brand"
  }

# Example Product
  • ProductTshirt
  {
    id=0,
    name="Midnite Sky",
    catalogId=3,
    price=75,
    productAttributes="XL;Black;Unisex;7artdesign"
  }
  
  # Example usage of GetProductsByAttr()
    • GetProductsByAttr("brand","7artdesign")
