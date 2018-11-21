<template>
    <div class="category-main">
        <div class="box">
            <div class="columns">
                <div class="column">
                     <p class="is-size-5">
                     <span class="icon is-small is-left">
                          <font-awesome-icon icon="dot-circle"></font-awesome-icon>  
                     </span>                    
                    Category</p>
                </div>   
                <div class="column is-one-quarter">
                    <div class="control is-rounded has-icons-right">                        
                        <input class="input" type="text" placeholder="Search">
                        <span class="icon is-small is-right">
                            <font-awesome-icon icon="search"></font-awesome-icon>                 
                        </span>            
                    </div>
                </div>                
            </div> 
            <div class="is-divider" data-content="OR"></div>
            <div class="field is-horizontal">
                <div class="field-label is-normal">
                    <p class="is-size-6">Crop ID</p>
                </div>
                <div class="field-body">
                    <div class="control">   
                        <div class="select">                        
                            <select>
                            <option>Select dropdown</option>
                            <option>With options</option>
                            </select>
                        </div>
                    </div>                   
                </div>
            </div>                                 
        </div> 
        <div class="field-section">
            <div class="field">
                <label class="label">Name</label>
                <div class="control">
                    <input class="input" type="text" placeholder="e.g Alex Smith">
                </div>
            </div>
            <div class="field">
                <label class="label">Email</label>
                <div class="control">
                    <input class="input" type="email" placeholder="e.g. alexsmith@gmail.com">
                </div>
            </div>       
        </div>        
    </div>
</template>
<script>
export default {
  layout: 'cms'
}``
</script>

<style>
.category-main {
  margin-right: 1rem;
}
.field-section {
  width: 400px;
}
</style>

