---
title: Partecipa all'evento
order: 7
include: sections/default.html
bg: bg-white

---

L'evento si terrà in presenza presso l'aula Giorgio Prodi, Piazza San Giovanni in Monte 2, Bologna. 
L'aula ha una capienza massima di 120 posti a sedere. Per partecipare, prenota il tuo posto registrandoti compilando il form.

<form id="attending-form" name="attending" method="POST" data-netlify="true">
    <div class="form-group">
        <label class="py-2" for="name"><b>Nome e Cognome</b></label>
        <input type="text" name="name" id="name" placeholder="Scrivi qui il tuo nome" class="form-control">   
    </div>
    <div class="form-group">
        <label class="py-2" for="email"><b>Email</b></label>
        <input type="email" name="email" id="email" autocomplete="email"  class="form-control" placeholder="Scrivi qui la tua email" title="The domain portion of the email address is invalid (the portion after the @)." pattern="^([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x22([^\x0d\x22\x5c\x80-\xff]|\x5c[\x00-\x7f])*\x22))*\x40([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d)(\x2e([^\x00-\x20\x22\x28\x29\x2c\x2e\x3a-\x3c\x3e\x40\x5b-\x5d\x7f-\xff]+|\x5b([^\x0d\x5b-\x5d\x80-\xff]|\x5c[\x00-\x7f])*\x5d))*(\.\w{2,})+$" required>
    </div>
    <div class="form-group">
        <label class="py-2" for="contest"><b>Sessione</b></label>
        <select name="session[]" class="form-select" aria-label="Default select example">
            <option selected>Seleziona qui la sessione/sessioni</option>
            <option value="prima-sessione">Prima sessione pomeridiana (De Mol, Di Cosmo)</option>
            <option value="seconda-sessione">Seconda sessione pomeridiana (Martini, Di Cosmo/Vitali)</option>
            <option value="prima-e-seconda-sessione">Prima + Seconda sessione pomeridiana</option>
        </select>
    </div>
    <button type="submit" name="submit" class="btn btn-secondary w-100 mt-2 pb-2">Invia la tua partecipazione</button>
</form>
