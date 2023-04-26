// A function to generate a random password
function generatePassword(length) {
  const charset = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*()_+~`|}{[]\:;?><,./-=";
  let password = "";
  for (let i = 0; i < length; i++) {
    password += charset.charAt(Math.floor(Math.random() * charset.length));
  }
  return password;
}

// Generate a 10-character password
console.log("10-character password: ", generatePassword(10));

// Generate a 15-character password
console.log("15-character password: ", generatePassword(15));

// Generate a 20-character password
console.log("20-character password: ", generatePassword(20));
