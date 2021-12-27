<template>
    <h1>A single user created!, with ID: {{  $route.params.id }}</h1>
</template>

<script>
export default{

    validate(data)
    {
      /*  console.log(data);
        return true; */

      //  return data.params.id == 1;

      return /^\d+$/.test(data.params.id)
    },
    layout : 'usersLayout'

}
</script>
