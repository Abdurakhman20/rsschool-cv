# Abdurakhman Usmanov

## Frontend Developer

## Contact Me:

- Phone: +7 (925) 952-31-42
- E-mail: ausmanov706@gmail.com
- Telegram: [Abdurakhman Usmanov](https://t.me/Ausm2002)
- Github: [Abdurakhman20](https://github.com/Abdurakhman20)

## About Me:

I am 20 years old. I am a student and in my free time I study web technologies. In the future, I want to become a real professional in the field of Frontend development.

## My Skills:

- HTML
- CSS / SCSS / TailwindCSS
- JavaScript (ES6+)
- TypeScript
- ReactJS
- Redux / Redux-Toolkit
- Git

## Code Examples:

```
export const maskPhoneNumber = (event: React.ChangeEvent<HTMLInputElement>) => {
  let value = event.target.value;
  let inputNumValue = value.replace(/\D/g, "");
  let formattedInputValue = "";
  const selectionStart = event.target.selectionStart;
  if (!inputNumValue) {
    return (event.target.value = "");
  }
  if (value.length !== selectionStart) {
    return;
  }
  if (["7", "8", "9"].indexOf(inputNumValue[0]) > -1) {
    //Russian phone number
    if (inputNumValue[0] === "9") {
      inputNumValue = "7" + inputNumValue;
    }
    const firstSymbol = inputNumValue[0] === "8" ? "+7" : "+7";
    formattedInputValue = firstSymbol + " ";

    if (inputNumValue.length > 1) {
      formattedInputValue += "(" + inputNumValue.substring(1, 4);
    }
    if (inputNumValue.length >= 5) {
      formattedInputValue += ") " + inputNumValue.substring(4, 7);
    }
    if (inputNumValue.length >= 8) {
      formattedInputValue += "-" + inputNumValue.substring(7, 9);
    }
    if (inputNumValue.length >= 10) {
      formattedInputValue += "-" + inputNumValue.substring(9, 11);
    }
  } else {
    // Not Russian phone number
    formattedInputValue = "+" + inputNumValue.substring(0, 16);
  }
  event.target.value = formattedInputValue;
};

```

## My Projects:

- React Sneakers: [GITHUB](https://github.com/Abdurakhman20/react-sneakers) \
  Technology stack: Javascript , React, React - Context, SCSS - Modules \
  Description: React-sneakers is a online store selling sneakers
- React Pizza: [GITHUB](https://github.com/Abdurakhman20/react-pizza) \
  Technology stack: Typescript , React, Redux-Toolkit, SCSS - Modules \
  Description: React-pizza is a online store selling pizzas

## Education:

- Moscow State University Of Civil Engineering
  - Information systems and technologies

## Languages:

- Russian: Native
- English: Pre-Intermediate (A2)
