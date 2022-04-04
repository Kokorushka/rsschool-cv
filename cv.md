# rsschool-cv

## Aleksandra Alekseeva

### Junior Frontend Developer

***

#### Contact information:


Phone: +7 926 895 55 99

E-mail: kokosha117@gmail.com

[Github](https://github.com/Kokorushka)

***

#### Briefly About Myself:

I have worked for about 7.5 years in the pharmaceutical industry, including almost 5 years in the field of clinical drug research. I decided to radically change the field of activity and apply my knowledge and skills in the IT industry.

I have mastered the frontend developer program on the Hexlet educational portal, simultaneously using other sources of information available to me on the profession of interest.

Thanks to my previous work experience, my soft-skills arsenal includes attention to detail, a passion for learning new things and a great desire to produce a useful product for people in the form of websites and applications.

***

#### Skills and Proficiency:

*  HTML5, CSS3
*  JavaScript, React 
*  Git, GitHub
*  VS Code, SublimeText
*  Figma, GIMP

***

#### Code example:

[**Let's Recycle! Kata from Codewars**](https://www.codewars.com/kata/5b6db1acb118141f6b000060)

You will be given a list of objects. Each object has type, material, and possibly secondMaterial. The existing materials are: paper, glass, organic, and plastic.

Your job is to sort these objects across the 4 recycling bins according to their material (and secondMaterial if it's present), by listing the type's of objects that should go into those bins.

```
function recycle(array) {
  const sorted = array.reduce((acc, item) => {
    const searched = item.material;
    acc[searched] = [...acc[searched], item.type];
    acc = {...acc,  [item.material]: acc[searched]};
    if (item.secondMaterial) {
      const secSearched = item.secondMaterial;
      acc[secSearched] = [...acc[secSearched], item.type];
      acc = {...acc,  [item.secondMaterial]: acc[secSearched]};
    }
    return acc;
  }, {'paper':[], 'glass': [], 'organic': [], 'plastic': []});
  return Object.values(sorted);
}
```

