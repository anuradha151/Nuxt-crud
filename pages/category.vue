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
            <hr>          
            <div class="level">
                <div class="field is-horizontal level-left">
                    <div class="field-label is-normal">
                        <p class="is-size-6" id="label-crop-id">Crop ID</p>
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
        </div>               
    </div>
</template>
<script>
export default {
  layout: 'cms'
}
</script>

<style>
.category-main {
  margin-right: 1rem;
}
.field-section {
  width: 400px;
}
#label-crop-id {
  width: 75px;
}
</style>

