# let contacts = [{
    name: "Maxwell Wright",
    phone: "(0191) 719 6495",
    email: "Curabitur.egestas.nunc@nonummyac.co.uk"
    }, {
    name: "Raja Villarreal",
    phone: "0866 398 2895",
    email: "posuere.vulputate@sed.com"
    }, {
    name: "Helen Richards",
    phone: "0800 1111",
    email: "libero@convallis.edu"
    }];
    
function showContacts(arr, ind) {
    if (arr instanceof Array) {
        if(!(ind instanceof Number)) {
            console.log(contacts[ind]);
        } else console.log("Please input number for index");
    } else console.log("Please input name of Array");
}

function showAllContacts(arr) {
    if (arr instanceof Array) {
        console.log(arr)
    } else console.log("Please input name of Array");
}

function addNewContact(arr, nm, phn, eml) {
    if (arr instanceof Array) {
        String(nm)
        if (!(phn===undefined || phn===null)) {
            if (!(eml===undefined || eml===null)) {
                let newContact = {name:nm};
                    newContact.phone = phn;
                    newContact.email = eml;
                contacts.push(newContact);
            } else console.log("Please input email");
        } else console.log("Please input digits for phone number");
    } else console.log("Please input name of Array");
}

