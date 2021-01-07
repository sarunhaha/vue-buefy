    <template>
        <section class="container has-text-left">
        <b-field label="Name">
        <b-input value="Kevin Garvey"></b-input>
        </b-field>

        <b-field label="Email" type="is-danger" message="This email is invalid">
        <b-input type="email" value="john@" maxlength="30"></b-input>
        </b-field>

        <b-field label="Username" type="is-success" message="This username is available">
        <b-input value="johnsilver" maxlength="30"></b-input>
        </b-field>
        </section>

        
    </template>
