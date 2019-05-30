<script>
  export let user;
</script>

<div
  class="shadow-lg leading-normal self-end bg-white rounded-lg m-10 relative">
  <div class="md:flex bg-white rounded-lg p-6">
    <img
      class="h-16 w-16 md:h-24 md:w-24 rounded-full mx-auto md:mx-0 md:mr-6"
      src={user.picture.medium}
      alt="Avatar" />
    <div class="text-center md:text-left">
      <h2 class="text-lg capitalize">{user.name.first} {user.name.last}!</h2>
      <div class="text-purple-500">User Profession</div>
      <div class="text-gray-600">{user.email}</div>
      <div class="text-gray-600">{user.cell}</div>

      <a href="javascript:;" class="btn btn-primary mt-2">Email</a>
    </div>
  </div>
</div>
